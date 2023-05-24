{% if type == 'basic' %}

{{data.cost|prefix: '**Cost:** '}}

{{data.quantityPerGearSlot|prefix: '**Quantity Per Gear Slot:** '}}

{% elif type == 'armor' %}

{{data.cost|prefix: '**Cost:** '}}

{{data.gearSlots|prefix: '**Gear Slots:** '}}

{{data.ac|prefix: '**AC:** '}}

{{data.properties|join: ', '|prefix: '**Properties:** '}}

{% elif type == 'weapon' %}

{{data.cost|prefix: '**Cost:** '}}

{{data.type|map: 'WeaponType'| prefix: '**Type:** '}}

{{data.range|map: 'Range'| prefix: '**Range:** '}}

{{data.damage|map: 'Damage'| prefix: '**Damage:** '}}

{{data.properties|map: 'WeaponProperty'| prefix: '**Properties:** '}}

{% elif type == 'magic' %}

{{data.bonus|prefix: '**Bonus.** '}}

{{data.benefit|prefix: '**Benefit.** '}}

{{data.curse|prefix: '**Curse.** '}}

{{data.personality|prefix: '**Personality.** '}}

{% endif %}