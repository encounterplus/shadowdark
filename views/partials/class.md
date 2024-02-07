{% if data.weapons %}
**{{'Class.Weapons'|l}}:** {{data.weapons}} 
{% endif %}

{% if data.armor %}
**{{'Class.Armor'|l}}:** {{data.armor}} 
{% endif %}

{% if data.hp %}
**{{'Common.HitPoints'|l}}:** {{data.hp}} 
{% endif %}

{% for feature in data.features %}
**{{feature.name}}.** {{feature.text}}
{% endfor %}