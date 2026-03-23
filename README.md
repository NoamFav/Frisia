# 🎯 Frisia

<div align="center">

<img src="https://img.shields.io/badge/java-23+-ED8B00.svg?style=for-the-badge&logo=openjdk" alt="Java">
<img src="https://img.shields.io/badge/javafx-23-blue.svg?style=for-the-badge" alt="JavaFX">
<img src="https://img.shields.io/badge/maven-3.9-red.svg?style=for-the-badge&logo=apachemaven" alt="Maven">
<img src="https://img.shields.io/badge/license-MIT-green.svg?style=for-the-badge" alt="License">

**Modern Frisian Draughts with advanced AI and multiplayer**

[Installation](#installation) · [How to Play](#how-to-play) · [Rules](#game-rules)

</div>

---

Frisia is a full-featured implementation of Frisian Draughts built with JavaFX — featuring multiple AI difficulty levels, local multiplayer, interactive tutorials, light/dark themes, and sound effects.

---

## Prerequisites

| Requirement | Version |
|-------------|---------|
| Java | 23+ |
| Maven | 3.8+ |
| JavaFX | 23 (included via Maven) |
| Graphics | OpenGL 2.1+ |

---

## Installation

```bash
git clone https://github.com/NoamFav/Frisia.git
cd Frisia
mvn clean javafx:run
```

**Package as installer:**
```bash
mvn clean package -Djpackage.type=dmg    # macOS
mvn clean package -Djpackage.type=exe    # Windows
mvn clean package -Djpackage.type=deb    # Linux
```

---

## How to Play

| Key | Action |
|-----|--------|
| Mouse click | Select and move pieces |
| Esc | Open game menu |
| M | Toggle sound |
| T | Switch theme (Light/Dark) |
| R | Restart |
| H | Show hint |
| Space | Pause AI thinking |

---

## Game Rules

Played on a **10×10 board**, dark squares only. Each player starts with **20 pieces**.

- **Pawns** move diagonally forward one square
- **Kings** move diagonally or orthogonally across multiple squares
- Captures are **mandatory** — multi-jump sequences allowed in any direction
- Win by eliminating all opponent pieces or blocking their moves
- Capture priority given to moves with the highest piece value

---

## Features

- Multiple AI difficulty levels (Minimax + alpha-beta pruning)
- Local multiplayer
- Five interactive tutorial lessons
- Light and dark themes
- Sound effects (toggleable)

---

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes and open a Pull Request

---

## License

MIT — see [LICENSE](LICENSE).

---

<div align="center">
Made with ❤️ by <a href="https://github.com/NoamFav">NoamFav</a>
</div>
