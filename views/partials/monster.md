{{data.ac | md-prefix: "AC"}}{{data.hp | prefix: "**HP** "}}
{{data.attacks | prefix: "**ATK** "}}
**S** {{data.str|signed|default: '+0'}}, **D** {{data.dex|signed|default: '+0'}}, **C** {{data.con|signed|default: '+0'}}, **I** {{data.int|signed|default: '+0'}}, **W** {{data.wis|signed|default: '+0'}}, **CH** {{data.cha|signed|default: '+0'}}
{{data.movement | md-prefix: "MV"}}{{data.alignment | md-prefix: "AL"}}{{data.level | md-prefix: "LV"}}
