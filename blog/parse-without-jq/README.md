# parse-without-jq

The "parse JSON and YAML without jq golf" demo from the OrchStep blog.

    orchstep run json_report   # JSON -> func: transform (JS)
    orchstep run yaml_report   # YAML -> result.data_object

Every step is a harmless `echo`/`printf`, so it runs anywhere.
