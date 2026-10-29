# Voice and wording

The wording rules and glossaries of each language in this pack. Loading and the file layout are in the
[README](../README.md).

## Spanish (es)

Locale `es` is neutral international Spanish: Latin American words that Spain also understands.

| English | es |
| --- | --- |
| computer | computadora |
| file | archivo |
| mobile phone | celular |
| email | correo electrónico |
| password | contraseña |
| settings | configuración |
| save | guardar |
| default | predeterminado |

Actions use the infinitive (Guardar, Cancelar). The `es` files do not use ordenador, fichero, móvil, vosotros, or voseo.

`EsRegional.xml` is a short overlay, not a second catalog:

- `es_ES`: fichero, móvil, and ajustes where the English is Settings. No label in this pass is Computer, so there is no ordenador row.
- `es_MX` has no rows of its own. archivo, celular, and configuración come from `es`.

These nine originals stay in `framework/data/CommonL10nData.xml` and are not repeated here: Add, Create, Delete, Description, Find, Name, Status, Type, Update.

A Spanish row is stored only when the text differs from the fallback: the original English, or the `default` template when one exists. A missing row returns that fallback. `es_MX` uses the `es` row.

Placeholders `${...}` and `{0}` `{1}` `{2}` `{3}` are copied unchanged. A `##` suffix stays on the key when its Spanish differs from the words before `##`. Strings longer than 255 characters cannot be keys.

## Simplified Chinese (zh)

Locale `zh` is Simplified Chinese, mainland UI wording, the same script as the `zh` rows in `CommonL10nData.xml`. There is no `zh_CN`, `zh_TW`, or `zh_HK` file. Traditional Chinese is a later catalog: a missing `zh_TW` row would fall back to Simplified `zh` before English.

The nine seed originals stay in `framework/data/CommonL10nData.xml` and are not repeated here.

Labels are short bare verbs (保存, 取消). Financial and GL account is 账户 (户, not 帐户). A login account is 账号. Shipment is 发货单. Party is 参与方. The token PO stays PO. Moqui, MR Moqui, Marble, and Mantle stay as written. `N/A` inside a template literal is 无.

| English | zh |
| --- | --- |
| Save | 保存 |
| Cancel | 取消 |
| Close | 关闭 |
| Submit | 提交 |
| Confirm | 确认 |
| Search | 搜索 |
| Edit | 编辑 |
| View | 查看 |
| Print | 打印 |
| Export | 导出 |
| Import | 导入 |
| New | 新建 |
| Copy | 复制 |
| Remove | 移除 |
| Settings | 设置 |
| File | 文件 |
| Email | 电子邮件 |
| Password | 密码 |
| User | 用户 |
| Username | 用户名 |
| Invoice | 发票 |
| Bill | 账单 |
| Order | 订单 |
| Purchase order | 采购订单 |
| Shipment | 发货单 |
| Party | 参与方 |
| Customer | 客户 |
| Supplier, Vendor | 供应商 |
| Employee | 员工 |
| Account (financial) | 账户 |
| Account (login) | 账号 |
| Accounting | 会计 |
| GL | 总账 |
| Payment | 付款 |
| Product | 产品 |
| Inventory | 库存 |
| Asset | 资产 |
| Facility | 设施 |
| Warehouse | 仓库 |
| Quantity | 数量 |
| Amount | 金额 |
| Price (unit) | 单价 |
| Active | 有效 |
| Cancelled | 已取消 |
| Completed | 已完成 |
| Approved | 已批准 |
| Pending | 待处理 |
| Draft | 草稿 |
| Mobile | 手机 |

Do not use 軟體, 資訊, 預設, 檔案, 設定, 網路, 程式 (程序 is the word; 方程式 may stay), 視窗, 螢幕, 滑鼠, 資料, or Cantonese 嘅 喺 唔 佢 咗 啲. Use 软件, 信息, 默认, 文件, 设置, 网络, 程序, 窗口, 屏幕, 鼠标, 数据.

A `zh` row is stored only when the text differs from the English original. The omitted originals are listed in `data/zh/unchanged-*.txt`, which the loader ignores. This pack follows the Spanish key set. A name that is spelled the same in English and Spanish, such as China or a province written in English, has no row in either pack, so a `zh` user still sees that English name. Placeholders `${...}` and `{0}` `{1}` `{2}` `{3}` are copied unchanged, including a `{n,choice,...}` pattern. Natural-language words inside a `${}` string literal are translated (`'No Lot #'`, `'N/A'`). A `##` inside a number pattern such as `#,##0.00` or `###-###` stays. The localized value is at most 255 characters.
