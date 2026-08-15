# 🌌 Aetheria

**Generador de mundos dimensionales con biomas customizados y estructuras procedurales para Terra/Minecraft.**

Aetheria es un pack de generación de mundos que expande las tres dimensiones clásicas (Overworld, Nether y End) con biomas únicos, fracturas dimensionales que conectan mundos, paletas de bloques detalladas y estructuras procedurales memorables.

---

## ✨ Características Principales

### 🌍 Tres Dimensiones Expandidas
- **Overworld**: 10+ biomas incluyendo Llanuras Agostadas (*Scorched Plains*) e Islas Flotantes (*Floating Isles*)
- **Nether**: 3 biomas raros — Paisajes Infernales Ardientes, Veldts Cristalinos y El Límite
- **End**: 5 biomas incluyendo Islas de Fractura Nether y Restos del Overworld

### 🔗 Fracturas Dimensionales
Sistema de fracturas que conectan las 3 dimensiones mediante estructuras especiales:
- **Puertas del Éter** (Overworld)
- **Grietas del Límite** (Nether)
- **Nexo de Fractura Dimensional** (End)

### 🎨 Sistema de Paletas
- **40+ paletas** organizadas por dimensión y bioma
- Paletas compartidas: piedra base, minerales, vegetación
- Soporte para altitud, temperatura y cobertura variable

### 🏛️ 30+ Estructuras Procedurales
Desde calabozos clásicos hasta estructuras dimensionales únicas:
- Overworld: 14 estructuras (templos, mansiones, naufragios, cámaras de pruebas...)
- Nether: 6 estructuras (bastiones, fortalezas, pilares de obsidiana...)
- End: 5 estructuras (ciudades, nexos, plataformas...)
- Dimensional: Puentes del Éter

---

## 📁 Estructura del Proyecto

```
Aetheria/
├── pack.yml                    # Configuración principal del pack
├── customization.yml           # Opciones de personalización del usuario
├── options.yml                 # Opciones técnicas y rarezas
├── README.md                   # Este archivo
│
├── biome-distribution/
│   ├── presets/
│   │   ├── default.yml
│   │   ├── overworld_focus.yml
│   │   ├── nether_focus.yml
│   │   └── end_focus.yml
│   └── stages/
│       ├── overworld_distribution.yml
│       ├── nether_distribution.yml
│       └── end_distribution.yml
│
├── biomes/
│   ├── colors.yml
│   ├── abstract/
│   │   └── base.yml
│   ├── overworld/
│   │   ├── land/
│   │   ├── aquatic/
│   │   ├── cave/
│   │   └── convergence/
│   ├── nether/
│   └── end/
│
├── palettes/
│   ├── shared/
│   │   ├── base_stone.yml
│   │   ├── ores.yml
│   │   └── vegetation.yml
│   ├── overworld/
│   │   ├── plains.yml
│   │   ├── forest.yml
│   │   ├── ocean.yml
│   │   ├── cave.yml
│   │   ├── mountain.yml
│   │   ├── river.yml
│   │   ├── desert.yml
│   │   ├── snow.yml
│   │   ├── jungle.yml
│   │   ├── swamp.yml
│   │   ├── mushroom.yml
│   │   ├── scorched_plains.yml
│   │   └── floating_isles.yml
│   ├── nether/
│   │   ├── basalt_deltas.yml
│   │   ├── crimson_forest.yml
│   │   ├── warped_forest.yml
│   │   ├── soul_sand_valley.yml
│   │   ├── nether_wastes.yml
│   │   ├── flaming_hellscapes.yml
│   │   ├── crystalline_veldts.yml
│   │   └── the_boundary.yml
│   └── end/
│       ├── main_island.yml
│       ├── outer_islands.yml
│       ├── chorus_forest.yml
│       ├── end_cities.yml
│       ├── netherfracture_isles.yml
│       ├── overworlx_remnants.yml
│       └── void.yml
│
├── structures/
│   ├── overworld/
│   │   ├── ruined_portal.yml
│   │   ├── ancient_ruins.yml
│   │   ├── floating_tower.yml
│   │   ├── crystal_shrine.yml
│   │   ├── aether_gates.yml
│   │   ├── dungeon.yml
│   │   ├── mineshaft.yml
│   │   ├── stronghold.yml
│   │   ├── desert_temple.yml
│   │   ├── jungle_temple.yml
│   │   ├── ocean_monument.yml
│   │   ├── woodland_mansion.yml
│   │   ├── pillager_outpost.yml
│   │   ├── village.yml
│   │   ├── shipwreck.yml
│   │   ├── ocean_ruin.yml
│   │   ├── trial_chamber.yml
│   │   └── trail_ruins.yml
│   ├── nether/
│   │   ├── bastion_remnant.yml
│   │   ├── nether_fortress.yml
│   │   ├── soul_spire.yml
│   │   ├── obsidian_pillar.yml
│   │   ├── boundary_rift.yml
│   │   ├── ruined_portal.yml
│   │   └── fossil.yml
│   ├── end/
│   │   ├── obsidian_platform.yml
│   │   ├── exit_portal.yml
│   │   └── dimensional_fracture_nexus.yml
│   └── dimensional/
│       └── aether_bridge.yml
│
├── features/
│   ├── overworld/
│   ├── nether/
│   └── end/
│
└── math/
    ├── functions/
    │   ├── terace.yml
    │   ├── lerp.yml
    │   └── maskSmooth.yml
    └── samplers/
        ├── samplex.yml
        ├── spots.yml
        └── fractureNoise.yml
```

---

## 🚀 Instalación

1. Descarga este repositorio como `.zip` o clónalo:
   ```bash
   git clone https://github.com/Bryan-Dev-PE/Aetheria.git
   ```

2. Coloca la carpeta `Aetheria/` en tu directorio de packs de Terra:
   ```
   plugins/Terra/packs/
   ```

3. Añade `Aetheria` a tu configuración de mundo en `config.yml`:
   ```yaml
   packs:
     - "Aetheria"
   ```

4. Reinicia el servidor o recarga Terra.

---

## ⚙️ Personalización

Edita `customization.yml` para ajustar el mundo a tu gusto:

| Opción | Descripción | Valor Default |
|--------|-------------|---------------|
| `overworld-biome-size` | Tamaño de biomas OW | `1.0` |
| `nether-biome-size` | Tamaño de biomas Nether | `1.0` |
| `end-preset` | Preset del End | `RINGS_OF_LIFE` |
| `fracture-overworld-nether` | Fracturas OW↔Nether | `true` |
| `fracture-intensity` | Intensidad de fracturas | `0.08` |

Edita `options.yml` para controlar rarezas y biomas desactivados.

---

## 📜 Licencia

Este proyecto está licenciado bajo la [MIT License](LICENSE).

---

## 👤 Autor

**Bryan-Dev-PE** — Creador y mantenedor del proyecto Aetheria.

> *"Entre el Éter y el Vacío, los mundos se fracturan."*