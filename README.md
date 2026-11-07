# Heronputt 1.0 TEST

Native Android Herugolf shrinking-shot puzzle. Android 8+ (min26), target35. Package com.gg007.heronputt.

## Rules
Tap ball A or B to select it, then use UP, RIGHT, DOWN or LEFT to take a shot. The first shot travels exactly the number printed on that ball: A starts at3, B at2. Each following shot is one cell shorter. Change direction only between shots; continuing straight is allowed. Land in an H hole to stop immediately, even before the distance falls to1. Every hole needs exactly one ball. Shots cannot pass over a hole, either starting tile, any existing trail or their own previous path. No crossing, overlapping, retracing or leaving the grid. Blue W cells are water: shots may cross water but cannot land there. A ball at zero without a hole cannot move; undo to recover. Empty floor may remain unused. Twelve unique4x4 layouts with two balls, two holes and two water cells. Every unique solution moves each ball at least twice and crosses water. Undo/reset/next/level selection and saved putt palette/shot-number settings.

## Download and status
https://mega.co.nz/#!tZFyDQ4K!ljdMMRIfANS9zYvbsZlfJPizbwz0UgfdHWpbsZ_STRU
APK SHA256 06e85c61cd5da448d7057984c10a029a47a8217dbd141cf479c372ad56c90876; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

Independent Java coordinate-range segment construction and visited-cell sets agree with production step-by-step ray walking on all1785 pairs of direction prefixes per board,21420 total, including incomplete routes. Position, remaining shot length, occupied trails, legal/illegal states and completion agree. Exactly one route-pair solution per board; twelve distinct route pairs. Bounds, invalid directions, solved-input lock, solve, undo and replay in both ball orders pass. Actual archived generator regeneration and archived Java tests pass. Drawing-adapter navigation, saved settings, privacy, ball selection, shot buttons, completion marks, next and level selection pass. Actual game/menu/settings/privacy/levels/solved drawing pixels inspected, not phone screenshots. Phone runtime, performance and external browser handoff QA remain incomplete. Signed TEST only, not final and not Play published.

## Functional difference
Live803-entry registry,117 recovered partial README records and semantic review of all143 cards in the exact Glowwillow cumulative stage found no Herugolf match. GolfMath calculates a sporting handicap, not a game. Potwillow sends circles along one straight route into sum pots; Heronputt makes multiple shots with strictly decreasing exact distances, changes direction at stops and distinguishes water crossing from water landing. Driftwell slides until a wall; these shots stop at fixed countdown distances. Cindertrail takes single-cell steps on one spark-collection route; this uses two independently selected balls, holes, reserved trails and shrinking segments. Known Herugolf genre, not a global invention. Corpus is partial. Rules verified at https://www.nikoli.co.jp/en/puzzles/herugolf/ and https://www.janko.at/Raetsel/Herugolf/index.htm .

## Build
JDK17 and Android SDK platform35/build-tools35.0.0. Run python generate-levels.py to reproduce levels.json. Board.java embeds the generated ball starts, shot lengths, holes, water and solutions. javac -d /tmp/heron-test src/com/gg007/heronputt/Board.java BoardTest.java and java -cp /tmp/heron-test com.gg007.heronputt.BoardTest. bash build.sh builds an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not a final store release.

## Privacy and branding
Heronputt runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Putt palette, shot numbers and completed-puzzle marks stay in the app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon copied byte-for-byte from preserved original. Menu includes studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation
Complete source and APK privately preserved at https://files.instinct.com/rk0vfub52q2y-heronputt-source-archive with exact cumulative staged HTML. GitHub https://github.com/iLanis-agent/heronputt holds README only; full Git source commit remains pending. Cumulative stage is NOT LIVE; existing studio run remains queued. No Pages settings changes, rollback or Play rollout. Updated November 7, 2026.
