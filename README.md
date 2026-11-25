# 科创企业订单现金缺口与融资接力

本项目用于整理相关业务资料。CSV 文件采用 UTF-8 编码，首行为字段名，日期使用 ISO 格式；空单元格表示来源未提供。样例记录为合成数据。

## 样例资料

- `orders.csv` 包含样例字段 `order,enterprise,customer,contract_value,delivery_date,acceptance_due,state`。
- `cash_events.csv` 包含样例字段 `event,order,kind,due_date,amount,confirmed`。
- `rd_spend.csv` 包含样例字段 `item,enterprise,period,kind,amount,budget_state`。
- `bank_offers.csv` 包含样例字段 `offer,bank,product,max_amount,max_months,security,eligible_proof`。

## 运行检查

需要 Python 3.11 或更高版本，无第三方依赖。

```bash
python3 -m unittest discover -s tests -v
python3 -m compileall -q tests
```
