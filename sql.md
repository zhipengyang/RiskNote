**1. 模型的特征集合**
```angular2html
select * from model_feature left join verify_feature on model_feature_feature_id=verify_feature_id where model_feature_model_id=90;
```

**2. 每个process的具体内容**
```angular2html
select * from task 
left join state on task_state_id=state_id
left join process on process_id=state_process_id
where process_id=27
```

**3. 查看节点耗时**
```angular2html
select distinct(node_consume_statistics_hours_state_id) , state_description from node_consume_statistics_hours
left join state on node_consume_statistics_hours_state_id = state_id
where node_consume_statistics_hours_apply_risk_source = 2
and node_consume_statistics_hours_apply_risk_source_apply_risk_type = 1
and 	node_consume_statistics_hours_sample_hours = '2018-01-06 15:00:00'
and state_process_id = 15
order by state_id
```

**4. 订单查询**
    select * from ticket where ticket_target_id=26235340;
    
    select * from task left join state on task_state_id=state_id left join process on process_id=state_process_id where process_id=26;
    
    select * from state where state_id=321;
    
    select * from process left join state on process_id=state_process_id where process_id=26;
    
    select * from verify_detail where verify_detail_apply_risk_id=26235340;
    
    select * from verify_detail where verify_detail_identity=441625199805274417;
    
    select * from apply_model_result where apply_model_result_risk_id=26235340;
    
    select * from verify_result where verify_result_id=30905201;
    
    select * from model_record where model_record_apply_risk_id=26235340;
    
    select * from tlog where tlog_ticket_id=26629045;
    
    select * from process where process_id=26;
    
    select * from state where state_process_id=26;
    
    select * from process left join state on process_id=state_process_id left join task on task_state_id=state_id where process_id=26;