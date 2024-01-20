{{data.ac | prefix: "**AC** "}} {{data.hp | prefix: "**HP** "}}
{{data.attacks | prefix: "**ATK** "}}
**S** {{data.str|default: 0|signed|roll: 'Strength'}}, **D** {{data.dex|default: 0|signed|roll: 'Dexterity'}}, **C** {{data.con|default: 0|signed|roll: 'Constitution'}}, **I** {{data.int|default: 0|signed|roll: 'Intelligence'}}, **W** {{data.wis|default: 0|signed|roll: 'Wisdom'}}, **CH** {{data.cha|default: 0|signed|roll: 'Charisma'}}
{{data.movement | prefix: "**MV** "}} {{data.alignment | prefix: "**AL** "}} {{data.level | prefix: "**LV** "}}