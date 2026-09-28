# Melo

Melo samlar en konsults dag i en Mac-app: dagsplan, mötesinspelning och protokoll, issues, körningar med Claude och
feedback, per kund.

## Installera

Kräver en Mac med Apple silicon (M1 eller senare) och macOS 26, att du är administratör på Macen, ett eget
Claude-abonnemang och ett GitHub-konto.

1. Ladda ner **[Melo.dmg](https://github.com/oliwerhelsen/melo-releases/releases/latest/download/Melo.dmg)**.
2. Öppna filen och dra Melo till Program.
3. Starta Melo. "Kom igång" leder dig resten av vägen:
   - **Installera vad som behövs**: Command Line Tools, Homebrew, gh, ffmpeg, whisper-cpp, uv, Claude Code,
     parakeet-mlx och de två transkriberingsmodellerna (ca 3 GB). macOS frågar efter ditt lösenord en gång.
   - **Claude-token**: kör `claude setup-token` och klistra in token.
   - **GitHub**: `gh auth login`.
   - **Första kunden** och en kort **testinspelning** så att macOS frågar om mikrofonen och ljudet.

Uppdateringar kommer av sig själva. "Sök efter uppdateringar…" i Melo-menyn letar direkt.

Vill du installera verktygen utan appen fungerar samma skript i Terminal: ladda ner `install.sh` från den senaste
releasen och kör `bash install.sh` (`--dry-run` visar vad det skulle göra).

## Vad som finns här

- `appcast.xml`: uppdateringsflödet som Melo läser (Sparkle).
- `install.sh`: samma installationsskript som ligger i appen.
- Releaser med `Melo.dmg`.

Källkoden är privat. Hittar du ett fel: Hjälp → Rapportera problem… i Melo.
