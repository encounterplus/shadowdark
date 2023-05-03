**HP** {{data.hpCurrent}} / {{data.hpMaximum}} **AC** {{data.ac}} **Level** {{data.level}} **XP** {{data.xp}}

**STR** {{data.str.base}} / {{data.str.mod|signed|default: '+0'}} **DEX** {{data.dex.base}} / {{data.dex.mod|signed|default: '+0'}} **CON** {{data.con.base}} / {{data.con.mod|signed|default: '+0'}}  
**INT** {{data.int.base}} / {{data.int.mod|signed|default: '+0'}} **WIS** {{data.wis.base}} / {{data.wis.mod|signed|default: '+0'}} **CHA** {{data.cha.base}} / {{data.cha.mod|default: '0'}}

{{data.ancestry|link: 'ancestry'|prefix: '**Ancestry** '}} {{data.class|link: 'class'|prefix: '**Class** '}} {{data.title|prefix: '**Title** '}} {{data.alignment|map: 'Alignment'|prefix: '**Alignment** '}} {{data.background|prefix: '**Background** '}} {{data.deity|prefix: '**Deity** '}}
