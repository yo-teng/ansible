# 使用說明
- 複製相對應設定檔

```bash
 cp inventory.instance.create.yml.example inventory.instance.create.yml
```
```bash
cp group_vars/all/env.yml.example group_vars/all/env.yml
```

- 調整並檢查以下檔案參數
```
  - group_vars/all/env.yml
  - vars/instance/instance_var.yml
  - vars/monitor/monitor_var.yml
```


- 執行
```
ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook -i inventory.instance.create.yml {task}
```
```
- 依照需求指定Task yaml
  - create_general_instance.yaml
