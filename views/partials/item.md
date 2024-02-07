{% if data.category == 'basic' %}

{% if data.cost %}
**{{'Item.Cost'|l}}:** {{data.cost}}
{% endif %}
{% if data.quantityPerGearSlot %}
**{{'Item.QuantityPerGearSlot'|l}}:** {{data.quantityPerGearSlot}}
{% endif %}

{% elif data.category == 'armor' %}

{% if data.cost %}
**{{'Item.Cost'|l}}:** {{data.cost}}
{% endif %}
{% if data.gearSlots %}
**{{'Item.GearSlot'|l}}:** {{data.gearSlots}}
{% endif %}
{% if data.ac %}
**{{'Common.AC'|l}}:** {{data.ac}}
{% endif %}
{% if data.properties %}
**{{'Item.Properties'|l}}:** {{data.properties|join: ', '}}
{% endif %}

{% elif data.category == 'weapon' %}

{% if data.cost %}
**{{'Item.Cost'|l}}:** {{data.cost}}
{% endif %}
{% if data.weaponType %}
**{{'Item.Type'|l}}:** {{data.weaponType|map: 'WeaponType'}}
{% endif %}
{% if data.range %}
**{{'Item.Range'|l}}:** {{data.range|map: 'Range'}}
{% endif %}
{% if data.damage %}
**{{'Item.Damage'|l}}:** {{data.damage|map: 'Damage'}}
{% endif %}
{% if data.properties %}
**{{'Item.Properties'|l}}:** {{data.properties|map: 'WeaponProperty'}}
{% endif %}

{% elif data.category == 'magic' %}

{% if data.bonus %}
**{{'Item.Bonus'|l}}.** {{data.bonus}}
{% endif %}
{% if data.benefit %}
**{{'Item.Benefit'|l}}.** {{data.benefit}}
{% endif %}
{% if data.curse %}
**{{'Item.Curse'|l}}.** {{data.curse}}
{% endif %}
{% if data.personality %}
**{{'Item.Personality'|l}}.** {{data.personality}}
{% endif %}

{% endif %}