\[to [SKILLS](/SKILLS.md)\]

**Flag (Флаг / Признак / Индикатор)** - Это обычно логическое значение, определяющее состояние чего-либо, например: признак активности записи, признак существования объекта и т.п. Иногда флагами или признаками или индикаторами могут называть не только логические т.е. boolean значние, но также и значения других типов, которы можно отнести к бинарному признаку `true` или  `false`. 

К пример часто можно встретить такие синонимы:
| boolean | numeric | char (Y/N) | char (T/F) |
|---------|---------|------------|------------|
| false   | 0       | N          | F          |
| true    | 1       | Y          | T          |

 ### Пример на Python
```python
isActive = True

if isActive:
	pass
```

 ### Пример на SQL
```SQL
select 
	   name, 
	   email, 
	   birtday_dt,
	   last_login_dttm,
	   CASE 
			WHEN last_login_dttm is not null THEN 'Y'
            ELSE 'N' 
	    END active_flg 

from User 
```

