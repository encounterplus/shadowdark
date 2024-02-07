{% if data.ac -%}**{{'Common.AC'|l}}** {{data.ac}} {% endif -%}
{% if data.hp -%}**{{'Common.HP'|l}}** {{data.hp}} {% endif -%}
{% if data.attacks %}
**{{'Common.ATK'|l}}** {{data.attacks}} 
{%- endif %}
**{{'Stat.S'|l}}** {{data.str|default: 0|signed|roll: 'Stat.Strength'}}, **{{'Stat.D'|l}}** {{data.dex|default: 0|signed|roll: 'Stat.Dexterity'}}, **{{'Stat.C'|l}}**{{data.con|default: 0|signed|roll: 'Stat.Constitution'}}, **{{'Stat.I'|l}}** {{data.int|default: 0|signed|roll: 'Stat.Intelligence'}}, **{{'Stat.W'|l}}** {{data.wis|default: 0|signed|roll: 'Stat.Wisdom'}}, **{{'Stat.CH'|l}}** {{data.cha|default: 0|signed|roll: 'Stat.Charisma'}}
{% if data.movement -%}**{{'Common.MV'|l}}** {{data.movement}} {% endif -%}
{% if data.alignment -%}**{{'Common.AL'|l}}** {{data.alignment}} {% endif -%}
{% if data.level -%}**{{'Common.LV'|l}}** {{data.level}} {% endif -%}