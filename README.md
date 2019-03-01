## 是什么

和小伙伴们一起通过Notion的表格页面协作记账，导出CSV之后，通过CSV自动计算个人需要支付/收取的费用。

## 怎么用
1. copy这个表格模板到自己的工作区 [表格模板](https://www.notion.so/9e7c374f18734d3e930bedb46c7fe8d6?v=adb94ec9338e4783a1c39de142729a32)
2. 和小伙伴一起用表格记账
3. 定期结算，导出表格，解压出CSV
4. `python bill.py bill.csv` 即可看到计算结果，A应该付给B多少费用。
    ```
    python bill.py ~/Desktop/-daa74600-754d-4356-9d6e-85f23494d66f.csv
    Mayne Yao需要向xx x收取2279.0649999999996
    xx x需要向Mayne Yao支付2279.0649999999996
    ```
5. 结算后将事项归档。
6. 重复2-5

## TODO
+ 通过链接直接计算结果
    ```
    python bill.py https://www.notion.so/9e7c374f18734d3e930bedb46c7fe8d6?v=adb94ec9338e4783a1c39de142729a32
    ```
    因为账单一般是不公开的，所以在使用前，现将账单设置为公共页面。计算后再次设置为私密（如果你不那么在意这部分隐私的话，也可以一直 share public）
    这样可以免去手动导出的步骤

+ 基于公开账单的web应用
    输入自己公开账单的链接即可结算。web版可以做更多可视化相关的操作，更加直观的认识到自己的消费情况。

## 如何copy模板
参见：[https://notionpages.com/how-to-copy-a-notion-template/](https://notionpages.com/how-to-copy-a-notion-template/)

