CqubeMetricTest is used to calculate the metrics of semester exception report, diksha stacked chart report, diksha column chart report and diksha table report.
Metrics test done by using the sql queries and json files(s3 output bucket json files).

Fill the Details in Database.ini

[pgsql] 
host= # hostname for connecting to postgres (ex :locahost or public ip) 
port=5432 # Port number for postgres (default port number is 5432)
database= # Enter the Database name for postgres which is provided in the config.yml while installing 
user= # Enter the username name for postgres which is provided in the config.yml while installing 
password= # Enter the password for postgres which is provided in the config.yml while installing

Fill the Details in json_data.ini

Download the output_data folder from the s3 output bucket and store in the home directory(ie /home/ubuntu/output_data).

[jsondata]
semester_exception_district_wise=/home/ubuntu/output_data/exception_list/semester_completion/district_sem_completion_2.json
semester_exception_block_wise=/home/ubuntu/output_data/exception_list/semester_completion/block_sem_completion_2.json
semester_exception_cluster_wise=/home/ubuntu/output_data/exception_list/semester_completion/cluster_sem_completion_2.json
semester_exception_school_wise=/home/ubuntu/output_data/exception_list/semester_completion/school_sem_completion_2.json

bar_chart_reports_course=/home/ubuntu/output_data/diksha_output/bar_chart_reports/course/*.json
bar_chart_reports_all=/home/ubuntu/output_data/diksha_output/bar_chart_reports/all/*.json
bar_chart_reports_textbook=/home/ubuntu/output_data/diksha_output/bar_chart_reports/textbook/*.json
bar_chart_reports_course_last_7_days=/home/ubuntu/output_data/diksha_output/bar_chart_reports/course/last_7_days/*.json
bar_chart_reports_all_last_7_days=/home/ubuntu/output_data/diksha_output/bar_chart_reports/all/last_7_days/*.json
bar_chart_reports_textbook_last_7_days=/home/ubuntu/output_data/diksha_output/bar_chart_reports/textbook/last_7_days/*.json
bar_chart_reports_course_last_30_days=/home/ubuntu/output_data/diksha_output/bar_chart_reports/course/last_30_days/*.json
bar_chart_reports_all_last_30_days=/home/ubuntu/output_data/diksha_output/bar_chart_reports/all/last_30_days/*.json
bar_chart_reports_textbook_last_30_days=/home/ubuntu/output_data/diksha_output/bar_chart_reports/textbook/last_30_days/*.json
bar_chart_reports_course_last_day=/home/ubuntu/output_data/diksha_output/bar_chart_reports/course/last_day/*.json
bar_chart_reports_all_last_day=/home/ubuntu/output_data/diksha_output/bar_chart_reports/all/last_day/*.json
bar_chart_reports_textbook_last_day=/home/ubuntu/output_data/diksha_output/bar_chart_reports/textbook/last_day/*.json

table_reports_course_last_7_days=/home/ubuntu/output_data/diksha_output/table_reports/course/last_7_days/*.json
table_reports_all_last_7_days=/home/ubuntu/output_data/diksha_output/table_reports/all/last_7_days/*.json
table_reports_textbook_last_7_days=/home/ubuntu/output_data/diksha_output/table_reports/textbook/last_7_days/*.json
table_reports_course_last_30_days=/home/ubuntu/output_data/diksha_output/table_reports/course/last_30_days/*.json
table_reports_all_last_30_days=/home/ubuntu/output_data/diksha_output/table_reports/all/last_30_days/*.json
table_reports_textbook_last_30_days=/home/ubuntu/output_data/diksha_output/table_reports/textbook/last_30_days/*.json
table_reports_course_last_day=/home/ubuntu/output_data/diksha_output/table_reports/course/last_day/*.json
table_reports_all_last_day=/home/ubuntu/output_data/diksha_output/table_reports/all/last_day/*.json
table_reports_textbook_last_day=/home/ubuntu/output_data/diksha_output/table_reports/textbook/last_day/*.json

stack_bar_reports_last_7_days=/home/ubuntu/output_data/diksha_output/stack_bar_reports/last_7_days/All.json
stack_bar_reports_last_30_day=/home/ubuntu/output_data/diksha_output/stack_bar_reports/last_30_days/All.json
stack_bar_reports_last_day=/home/ubuntu/output_data/diksha_output/stack_bar_reports/last_day/All.json
stack_bar_reports_last_7_day=/home/ubuntu/output_data/diksha_output/stack_bar_reports/last_7_days/*.json
stack_bar_reports_last_30_days=/home/ubuntu/output_data/diksha_output/stack_bar_reports/last_30_days/*.json
stack_bar_reports_last_days=/home/ubuntu/output_data/diksha_output/stack_bar_reports/last_day/*.json

exception_list=/home/ubuntu/output_data/exception_list/school_invalid_data.json

Run the test script by using the run_tests.py

Location of the file CqubeMetric -> RunTestScripts -> run.tests.py

Note : Recommended Environment for running the test scripts are ubuntu 18.0.4.LTS or above and open the Project in the Pycharm IDE.
