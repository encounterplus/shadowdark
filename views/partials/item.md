{% if data.category == 'basic' %}

{{data.cost|prefix: '**Cost:** '}}

{{data.quantityPerGearSlot|prefix: '**Quantity Per Gear Slot:** '}}

{% elif data.category == 'armor' %}

{{data.cost|prefix: '**Cost:** '}}

{{data.gearSlots|prefix: '**Gear Slots:** '}}

{{data.ac|prefix: '**AC:** '}}

{{data.properties|join: ', '|prefix: '**Properties:** '}}

{% elif data.category == 'weapon' %}

{{data.cost|prefix: '**Cost:** '}}

{{data.weaponType|map: 'WeaponType'| prefix: '**Type:** '}}

{{data.range|map: 'Range'| prefix: '**Range:** '}}

{{data.damage|map: 'Damage'| prefix: '**Damage:** '}}

{{data.properties|map: 'WeaponProperty'| prefix: '**Properties:** '}}

{% elif data.category == 'magic' %}

{{data.bonus|prefix: '**Bonus.** '}}

{{data.benefit|prefix: '**Benefit.** '}}

{{data.curse|prefix: '**Curse.** '}}

{{data.personality|prefix: '**Personality.** '}}

{% endif %}