---
order: 6
zh-CN:
	title: 支持设置 Dialog 中的 button 类型
	content: 确认删除吗？
	title1: 请确认
	confirm: 删除
	cancel: 取消
	button: 删除
en-US:
	title: The type of button in Dialog is settable.
	content: Confirm to delete?
	title1: Confirm.
	confirm: Delete
	cancel: Cancel
	button: Dialog before delete sth.
---

```js
import { Sweetalert, Button } from 'zent';

const showAlertInfo = () => {
	Sweetalert.confirm({
		confirmType: 'danger',
		confirmText: '{i18n.confirm}',
		cancelText: '{i18n.cancel}',
		content: '{i18n.content}',
		title: '{i18n.title1}'
	});
}

ReactDOM.render(
	<Button onClick={showAlertInfo} type="danger">{i18n.button}</Button>,
	mountNode
);
```
