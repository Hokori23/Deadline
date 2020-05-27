# Deadline
A Project that record deadlines

## Features

 > 基本逻辑
 - 可以分组建立作业板
 - 每个组有唯一字段--group_id
 - 用户可通过唯一字段group_id申请加入组内，请求会进入请求队列中（保存于数据库中）
 - 组内由管理员通过检测请求队列来批准请求
 - 管理员可以通过user_id邀请用户，也会有一个请求队列保存这些邀请请求
 - 组内分权：
      - 0 -- 只可查看；
      - 1 -- 可编辑Deadline；
      - 2 -- 可编辑Deadline，可编辑Deadline类型，可邀请用户，可批准用户小组申请
      
 > 视图层
 1. y轴为Deadline类型、x轴为时间
 2. 日历形式，角落有事件备注颜色，
