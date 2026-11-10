# Quests & Progression for Godot

[Product and downloads](https://fableweld-labs.itch.io/quests-progression) · [Bug reports](https://github.com/fableweldlabs/fableweldlabs/issues)

Version 0.1.0. Regular price $9.99 USD; see the product page for the current launch discount. The addon is 258,216 bytes. Editable Lumen Vale and the free Windows demo are optional separate downloads.

**Supported engine requirement:** use the supplied modified Godot 4.7.2 Windows x86_64 editor and matching template. It is not an official Godot release. Stock 4.7.2 has a recorded intermittent full-world shutdown failure; this release does not claim full stock-engine compatibility or support for other versions/platforms. The modified engine is a separate free download.

Stable-ID quests and objectives, prerequisites, direct XP or event rewards, journal filters, tracker, timers, repeat/retry, optional/hidden objectives, actor hand-in and confirmed abandonment. Quest-only reviewed ID-renaming writes a separate save copy; component checkpoints are not universal whole-game saves. Connected generators require their documented separately licensed dependencies and exact supported versions. No complete RPG kit is bundled.

Conventional Light/Dark themes, optional Fableweld/Gold, saved 100/125/150% text sizes, Find action and focus scrolling. Twelve interface/example/quick-start languages; English fallback. Translations were prepared with AI assistance and have not had independent native-speaker certification.

For support include product/version, exact engine build, OS and reproduction steps. Do not post paid source or private project files publicly. Private support: fableweldlabs@gmail.com. Copyright 2026 Gordon Hinchen; Fableweld Labs branding. Product license and exact component notices are supplied with each download.

# Quick start / Guía rápida / Guia rápido / 快速开始 / クイックスタート / Démarrage rapide

[English](#en) · [Español](#es) · [Português (Brasil)](#pt_br) · [简体中文](#zh_cn) · [日本語](#ja) · [Français](#fr) · [Deutsch](#de) · [Polski](#pl) · [한국어](#ko) · [繁體中文](#zh_tw) · [Türkçe](#tr) · [Українська](#uk)

<a id="en"></a>

## English

For this release, use the separately supplied Fableweld corrected Godot 4.7.2 build. Unmodified 4.7.2 may crash during shutdown. See [Engine scope](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md); the portable editor is supplied separately for this release.

Optional Inventory 1.0: choose **Prepare Inventory compatibility**, review and confirm, then save, close and reopen the project before generating the Inventory example. Keep `res://fableweld_compatibility/inventory-1.0.0/` with your project backup. Modified or unsupported provider files are refused.

1. Back up your Godot project. Copy `addons/fableweld_quests` into its `addons` folder. Enable **Fableweld Quests** in Project Settings > Plugins.
2. In the Fableweld Quests dock, choose a language and quest preset, then press **Add preset quest**. Apply or revert pending fields before changing selection.
3. Edit the quest and objective, then press **Apply quest**. Create `res://game_data` and `res://gameplay`. Choose `res://game_data/quests.tres` for the catalog and press **Save**.
4. Choose a fresh scene path such as `res://gameplay/quest_playground.tscn`. Press **Create playable example**, open the new scene and run it with F6. Existing scene files are preserved.
5. Accept a quest before advancing its matching objectives. Simulation buttons are developer controls. To try combat, install the matched Combat dependency and use **Create connected Combat example**; accept Garden patrol, resolve enemy turns and claim XP after victory.
6. Use the language picker, then save and restore progress. A standard scene saves quests and its configured character; the Combat example also saves its fight. Other world state is excluded. Use a different save slot for independent progress.

For direct XP, set a quest reward, leave its reward event empty and apply the quest before generating. Complete the quest and claim once. Generated catalogs/profiles are copies; later dock edits do not update an existing scene.

Stop the game, disable the plugin and close the editor before updating. Replace only `addons/fableweld_quests`; preserve script UIDs, creator resources/scenes and saves. Test in a backup copy. Changed IDs/content may refuse old saves; no automatic migration is promised.

Use the current coordinated candidate archives. The historical review ZIP predates this guide. See [Optional dependencies](DEPENDENCIES.md). Public release is not authorized.

<a id="es"></a>

## Español

Para esta versión, usa la compilación corregida de Godot 4.7.2 de Fableweld, suministrada por separado. La versión 4.7.2 sin modificar puede fallar al cerrarse. Consulta [Alcance del motor](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md); el editor portátil se suministra por separado para esta versión.

Inventory 1.0 opcional: elige **Preparar compatibilidad de inventario**, revisa y confirma; guarda, cierra y vuelve a abrir el proyecto antes de generar el ejemplo. Conserva `res://fableweld_compatibility/inventory-1.0.0/` con la copia del proyecto. Se rechazan archivos modificados o no compatibles.

1. Haz una copia de seguridad del proyecto Godot. Copia `addons/fableweld_quests` a su carpeta `addons`. Activa **Fableweld Quests** en Ajustes del proyecto > Plugins.
2. En el panel Fableweld Quests, elige idioma y preajuste de misión; pulsa **Añadir misión predefinida**. Aplica o revierte los campos pendientes antes de cambiar la selección.
3. Edita la misión y su objetivo; pulsa **Aplicar misión**. Crea `res://game_data` y `res://gameplay`. Elige `res://game_data/quests.tres` para el catálogo y pulsa **Guardar**.
4. Elige una ruta nueva, como `res://gameplay/quest_playground.tscn`. Pulsa **Crear ejemplo jugable**, abre la escena y ejecútala con F6. Los archivos existentes se conservan.
5. Acepta una misión antes de avanzar sus objetivos. Los botones de simulación son herramientas de desarrollo. Para probar combate, instala la dependencia compatible y usa **Crear ejemplo de combate conectado**; acepta Patrulla del jardín, resuelve los turnos enemigos y reclama EXP tras ganar.
6. Usa el selector de idioma y guarda y restaura el progreso. Una escena normal guarda misiones y el personaje configurado; el ejemplo de combate también guarda la batalla. El resto del mundo queda fuera. Usa otra ranura para progreso independiente.

Para EXP directa, configura la recompensa, deja vacío el evento de recompensa y aplica la misión antes de generar. Completa y reclama una vez. Los catálogos y perfiles generados son copias; los cambios posteriores del panel no actualizan la escena.

Antes de actualizar, detén el juego, desactiva el plugin y cierra el editor. Sustituye solo `addons/fableweld_quests`; conserva UID, recursos, escenas y partidas. Prueba en una copia. Cambiar IDs o contenido puede invalidar una partida; no se promete migración automática.

Usa los archivos candidatos coordinados actuales. El ZIP histórico de revisión es anterior a esta guía. Consulta [Dependencias opcionales](DEPENDENCIES.md). La publicación no está autorizada.

<a id="pt_br"></a>

## Português (Brasil)

Para esta versão, use a versão corrigida do Godot 4.7.2 da Fableweld, fornecida separadamente. A versão 4.7.2 original pode falhar ao encerrar. Veja [Escopo do motor](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md); o editor portátil é fornecido separadamente para esta versão.

Inventory 1.0 opcional: escolha **Preparar compatibilidade do inventário**, revise e confirme; salve, feche e reabra o projeto antes de gerar o exemplo. Guarde `res://fableweld_compatibility/inventory-1.0.0/` junto ao backup do projeto. Arquivos alterados ou incompatíveis são recusados.

1. Faça uma cópia de segurança do projeto Godot. Copie `addons/fableweld_quests` para a pasta `addons`. Ative **Fableweld Quests** em Configurações do projeto > Plugins.
2. No painel Fableweld Quests, escolha idioma e predefinição de missão; pressione **Adicionar missão predefinida**. Aplique ou reverta campos pendentes antes de mudar a seleção.
3. Edite a missão e o objetivo; pressione **Aplicar missão**. Crie `res://game_data` e `res://gameplay`. Escolha `res://game_data/quests.tres` para o catálogo e pressione **Salvar**.
4. Escolha um caminho novo, como `res://gameplay/quest_playground.tscn`. Pressione **Criar exemplo jogável**, abra a cena e execute com F6. Arquivos existentes são preservados.
5. Aceite uma missão antes de avançar objetivos correspondentes. Botões de simulação são ferramentas de desenvolvimento. Para combate, instale a dependência compatível e use **Criar exemplo de combate conectado**; aceite Patrulha do jardim, resolva turnos inimigos e receba EXP após vencer.
6. Use o seletor de idioma, salve e restaure o progresso. Uma cena comum salva missões e o personagem configurado; o exemplo de combate também salva a luta. Outros estados do mundo ficam fora. Use outro espaço de salvamento para progresso independente.

Para EXP direta, defina a recompensa, deixe o evento de recompensa vazio e aplique a missão antes de gerar. Complete e receba uma vez. Catálogos e perfis gerados são cópias; alterações posteriores no painel não atualizam a cena.

Antes de atualizar, pare o jogo, desative o plugin e feche o editor. Substitua apenas `addons/fableweld_quests`; preserve UIDs, recursos, cenas e salvamentos. Teste numa cópia. Mudanças de IDs ou conteúdo podem recusar salvamentos antigos; não há migração automática garantida.

Use os arquivos candidatos coordenados atuais. O ZIP histórico de revisão é anterior a este guia. Consulte [Dependências opcionais](DEPENDENCIES.md). A publicação não está autorizada.

<a id="zh_cn"></a>

## 简体中文

本版本请使用单独提供的 Fableweld 修正版 Godot 4.7.2。未经修改的 4.7.2 可能在退出时崩溃。请参阅[引擎适用范围](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md)；本版本单独提供便携式编辑器。

可选 Inventory 1.0：选择 **准备背包兼容配置**，检查并确认，然后保存、关闭并重新打开项目，再生成背包示例。请将 `res://fableweld_compatibility/inventory-1.0.0/` 与项目备份一起保留。修改过或不受支持的提供方文件将被拒绝。

1. 先备份 Godot 项目。将 `addons/fableweld_quests` 复制到项目的 `addons` 文件夹，在项目设置 > 插件中启用 **Fableweld Quests**。
2. 在 Fableweld Quests 面板中选择语言和任务预设，然后点击 **添加预设任务**。切换选择前，先应用或还原尚未提交的字段。
3. 编辑任务和目标，点击 **应用任务**。创建 `res://game_data` 和 `res://gameplay` 文件夹。将目录路径设为 `res://game_data/quests.tres`，点击 **保存**。
4. 选择新的场景路径，例如 `res://gameplay/quest_playground.tscn`。点击 **创建试玩示例**，打开新场景并按 F6 运行。已有场景文件会保留。
5. 先接受任务，再推进对应目标。模拟按钮仅用于开发测试。要体验战斗，请安装匹配的战斗依赖并点击 **创建关联战斗示例**；接受花园巡逻任务，执行敌方回合，获胜后领取经验。
6. 使用语言选择器，然后保存和恢复进度。普通场景保存任务和已配置角色；战斗示例还保存战斗。其他世界状态不包含在内。独立进度应使用不同存档槽。

若要直接奖励经验，请设置任务经验奖励，将奖励事件留空，应用任务后再生成场景。完成后领取一次。生成的目录和配置是副本；面板之后的修改不会自动更新已有场景。

更新前停止游戏、禁用插件并关闭编辑器。只替换 `addons/fableweld_quests`，保留脚本 UID、创作资源、场景和存档。先在备份副本中测试。修改 ID 或内容可能导致旧存档被拒绝；不保证自动迁移。

请使用当前配套的候选安装包。历史审阅 ZIP 早于本指南。请参阅[可选依赖](DEPENDENCIES.md)。尚未授权公开发布。

<a id="ja"></a>

## 日本語

このリリースでは、別途提供される Fableweld 修正版 Godot 4.7.2 を使用してください。未修正の 4.7.2 は終了時にクラッシュする場合があります。[エンジンの対応範囲](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md)を確認してください。このリリースにはポータブルエディターが別途付属します。

任意の Inventory 1.0：**インベントリ互換性を準備** を選択して内容を確認し、承認します。保存後にプロジェクトを閉じて開き直してから例を生成してください。`res://fableweld_compatibility/inventory-1.0.0/` はプロジェクトのバックアップと共に保持してください。変更済み・非対応の提供元ファイルは拒否されます。

1. Godot プロジェクトをバックアップします。`addons/fableweld_quests` をプロジェクトの `addons` にコピーし、プロジェクト設定 > プラグインで **Fableweld Quests** を有効にします。
2. Fableweld Quests ドックで言語とクエストプリセットを選び、**プリセットのクエストを追加** を押します。選択を変える前に、未適用の入力を適用または元に戻してください。
3. クエストと目標を編集し、**クエストを適用** を押します。`res://game_data` と `res://gameplay` を作成します。カタログの保存先を `res://game_data/quests.tres` にして **保存** を押します。
4. `res://gameplay/quest_playground.tscn` など新しいシーンパスを指定します。**試遊サンプルを作成** を押し、シーンを開いて F6 で実行します。既存のシーンファイルは保持されます。
5. 対応する目標を進める前にクエストを受注します。シミュレーションボタンは開発用です。戦闘を試す場合は対応する依存機能を導入し、**接続済み戦闘サンプルを作成** を使います。庭園の巡回を受注し、敵のターンを進め、勝利後に経験値を受け取ります。
6. 言語を切り替え、進行を保存・復元します。通常のシーンはクエストと設定済みキャラクターを、戦闘サンプルは戦闘も保存します。他のワールド状態は対象外です。独立した進行には別の保存スロットを使ってください。

経験値を直接与えるには、報酬経験値を設定し、報酬イベントを空にして適用してからシーンを生成します。完了後に一度受け取れます。生成したカタログやプロファイルはコピーです。後からのドック編集は既存シーンに自動反映されません。

更新前にゲームを停止し、プラグインを無効にしてエディターを閉じます。`addons/fableweld_quests` だけを置き換え、UID、制作リソース、シーン、セーブを保持します。コピーで試してください。ID や内容の変更で旧セーブが拒否される場合があり、自動移行は保証されません。

現在の対応する候補アーカイブを使用してください。過去のレビュー ZIP はこのガイドより古いものです。[任意の依存関係](DEPENDENCIES.md)を参照してください。公開は許可されていません。

<a id="fr"></a>

## Français

Pour cette version, utilisez la version corrigée de Godot 4.7.2 par Fableweld, fournie séparément. La version 4.7.2 non modifiée peut planter à la fermeture. Consultez la [portée du moteur](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md) ; l’éditeur portable est fourni séparément pour cette version.

Inventory 1.0 facultatif : choisissez **Préparer la compatibilité Inventaire**, vérifiez et confirmez, puis enregistrez, fermez et rouvrez le projet avant de générer l’exemple. Conservez `res://fableweld_compatibility/inventory-1.0.0/` avec la sauvegarde du projet. Les fichiers modifiés ou non pris en charge sont refusés.

1. Sauvegardez le projet Godot. Copiez `addons/fableweld_quests` dans son dossier `addons`. Activez **Fableweld Quests** dans Paramètres du projet > Extensions.
2. Dans le panneau Fableweld Quests, choisissez la langue et un modèle de quête, puis **Ajouter une quête prédéfinie**. Appliquez ou annulez les champs en attente avant de changer la sélection.
3. Modifiez la quête et son objectif, puis **Appliquer la quête**. Créez `res://game_data` et `res://gameplay`. Choisissez `res://game_data/quests.tres` pour le catalogue et **Sauvegarder**.
4. Choisissez un nouveau chemin, par exemple `res://gameplay/quest_playground.tscn`. Utilisez **Créer un exemple jouable**, ouvrez la scène et lancez-la avec F6. Les fichiers existants sont conservés.
5. Acceptez une quête avant de faire progresser ses objectifs. Les boutons de simulation servent au développement. Pour le combat, installez la dépendance compatible et utilisez **Créer un exemple de combat connecté** ; acceptez Patrouille du jardin, jouez les tours adverses et réclamez les XP après la victoire.
6. Changez de langue, puis sauvegardez et restaurez. Une scène standard conserve quêtes et personnage configuré ; le combat conserve aussi la bataille. Les autres états du monde sont exclus. Utilisez un autre emplacement pour une progression indépendante.

Pour des XP directs, définissez la récompense, laissez son événement vide et appliquez la quête avant de générer. Terminez et réclamez une fois. Catalogues et profils générés sont des copies ; les changements ultérieurs du panneau ne modifient pas la scène existante.

Avant une mise à jour, arrêtez le jeu, désactivez l’extension et fermez l’éditeur. Remplacez uniquement `addons/fableweld_quests` ; conservez UID, ressources, scènes et sauvegardes. Testez sur une copie. Des ID ou contenus modifiés peuvent faire refuser les anciennes sauvegardes ; aucune migration automatique n’est promise.

Utilisez les archives candidates coordonnées actuelles. L’ancien ZIP de révision précède ce guide. Consultez les [dépendances facultatives](DEPENDENCIES.md). La publication n’est pas autorisée.

<a id="de"></a>

## Deutsch

Für diese Veröffentlichung den separat bereitgestellten, korrigierten Godot-4.7.2-Build von Fableweld verwenden. Die unveränderte Version 4.7.2 kann beim Beenden abstürzen. Siehe [Engine-Geltungsbereich](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md); der portable Editor wird für diese Veröffentlichung separat bereitgestellt.

Optionales Inventory 1.0: **Inventarkompatibilität vorbereiten** wählen, prüfen und bestätigen. Dann speichern, das Projekt schließen und vor der Beispielerstellung neu öffnen. `res://fableweld_compatibility/inventory-1.0.0/` mit der Projektsicherung aufbewahren. Geänderte oder nicht unterstützte Anbieterdateien werden abgewiesen.

1. Sichere dein Godot-Projekt. Kopiere `addons/fableweld_quests` in den Ordner `addons`. Aktiviere **Fableweld Quests** unter Projekteinstellungen > Plugins.
2. Wähle im Dock Fableweld Quests eine Sprache und Questvorlage und drücke **Vorlagenquest hinzufügen**. Wende offene Eingaben an oder verwerfe sie, bevor du die Auswahl änderst.
3. Bearbeite Quest und Ziel und drücke **Quest anwenden**. Erstelle `res://game_data` und `res://gameplay`. Wähle `res://game_data/quests.tres` für den Katalog und drücke **Speichern**.
4. Wähle einen neuen Szenenpfad, etwa `res://gameplay/quest_playground.tscn`. Drücke **Spielbares Beispiel erstellen**, öffne die Szene und starte sie mit F6. Vorhandene Szenendateien bleiben erhalten.
5. Nimm die Quest an, bevor du passende Ziele voranbringst. Simulationsknöpfe dienen der Entwicklung. Installiere für Kämpfe die passende Abhängigkeit und nutze **Verbundenes Kampfbeispiel erstellen**. Nimm Gartenpatrouille an, führe Gegnerzüge aus und hole nach dem Sieg die EP ab.
6. Wechsle die Sprache, speichere und lade den Fortschritt. Eine normale Szene speichert Quests und den eingerichteten Charakter; das Kampfbeispiel auch den Kampf. Anderer Weltzustand ist ausgeschlossen. Nutze für unabhängigen Fortschritt einen anderen Speicherplatz.

Für direkte EP legst du die Belohnung fest, lässt das Belohnungsereignis leer und wendest die Quest vor dem Erzeugen an. Schließe sie ab und hole die Belohnung einmal ab. Erzeugte Kataloge und Profile sind Kopien; spätere Dockänderungen aktualisieren bestehende Szenen nicht.

Stoppe vor einem Update das Spiel, deaktiviere das Plugin und schließe den Editor. Ersetze nur `addons/fableweld_quests`; erhalte UIDs, eigene Ressourcen, Szenen und Spielstände. Teste in einer Kopie. Geänderte IDs oder Inhalte können alte Spielstände ablehnen; automatische Migration ist nicht zugesagt.

Verwenden Sie die aktuellen aufeinander abgestimmten Kandidatenarchive. Das historische Prüf-ZIP ist älter als diese Anleitung. Siehe [Optionale Abhängigkeiten](DEPENDENCIES.md). Die Veröffentlichung ist nicht genehmigt.

<a id="pl"></a>

## Polski

W tej wersji użyj poprawionej kompilacji Godot 4.7.2 od Fableweld, dostarczonej oddzielnie. Niezmieniona wersja 4.7.2 może ulec awarii podczas zamykania. Zobacz [zakres obsługi silnika](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md); przenośny edytor jest dostarczany oddzielnie do tej wersji.

Opcjonalne Inventory 1.0: wybierz **Przygotuj zgodność ekwipunku**, sprawdź i potwierdź, a następnie zapisz, zamknij i otwórz projekt ponownie przed utworzeniem przykładu. Zachowaj `res://fableweld_compatibility/inventory-1.0.0/` razem z kopią projektu. Zmienione lub nieobsługiwane pliki dostawcy są odrzucane.

1. Utwórz kopię zapasową projektu Godot. Skopiuj `addons/fableweld_quests` do folderu `addons`. Włącz **Fableweld Quests** w Ustawieniach projektu > Wtyczki.
2. W panelu Fableweld Quests wybierz język i szablon zadania, a następnie **Dodaj gotowe zadanie**. Przed zmianą wyboru zastosuj albo odrzuć oczekujące pola.
3. Edytuj zadanie i cel, a następnie **Zastosuj zadanie**. Utwórz `res://game_data` i `res://gameplay`. Wybierz `res://game_data/quests.tres` jako katalog i **Zapisz**.
4. Wybierz nową ścieżkę, np. `res://gameplay/quest_playground.tscn`. Użyj **Utwórz grywalny przykład**, otwórz scenę i uruchom ją klawiszem F6. Istniejące pliki pozostaną bez zmian.
5. Przyjmij zadanie przed wykonywaniem pasujących celów. Przyciski symulacji służą do testów deweloperskich. Aby sprawdzić walkę, zainstaluj zgodną zależność i użyj **Utwórz połączony przykład walki**. Przyjmij Patrol ogrodu, rozegraj tury przeciwnika i odbierz PD po zwycięstwie.
6. Zmień język, zapisz i odczytaj postęp. Zwykła scena zapisuje zadania i skonfigurowaną postać; przykład walki również bitwę. Inny stan świata nie jest objęty zapisem. Dla niezależnego postępu wybierz inne miejsce zapisu.

Dla bezpośrednich PD ustaw nagrodę, pozostaw zdarzenie nagrody puste i zastosuj zadanie przed generowaniem. Ukończ je i odbierz nagrodę raz. Wygenerowane katalogi i profile są kopiami; późniejsze zmiany panelu nie aktualizują istniejącej sceny.

Przed aktualizacją zatrzymaj grę, wyłącz wtyczkę i zamknij edytor. Wymień tylko `addons/fableweld_quests`; zachowaj UID, własne zasoby, sceny i zapisy. Testuj w kopii. Zmiana ID lub treści może spowodować odrzucenie starych zapisów; automatyczna migracja nie jest gwarantowana.

Użyj bieżących, zgodnych archiwów kandydujących. Historyczny ZIP przeglądowy jest starszy od tej instrukcji. Zobacz [Opcjonalne zależności](DEPENDENCIES.md). Publikacja nie jest autoryzowana.

<a id="ko"></a>

## 한국어

이번 릴리스에는 별도로 제공되는 Fableweld 수정 Godot 4.7.2 빌드를 사용하세요. 수정되지 않은 4.7.2는 종료 중 충돌할 수 있습니다. [엔진 지원 범위](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md)를 확인하세요. 이 릴리스용 휴대용 편집기는 별도로 제공됩니다.

선택 사항인 Inventory 1.0: **인벤토리 호환성 준비**를 선택하고 검토 및 확인한 뒤, 프로젝트를 저장하고 닫았다가 다시 열어 예제를 생성하세요. `res://fableweld_compatibility/inventory-1.0.0/`를 프로젝트 백업과 함께 보관하세요. 수정되었거나 지원되지 않는 제공자 파일은 거부됩니다.

1. Godot 프로젝트를 백업하세요. `addons/fableweld_quests`를 프로젝트의 `addons` 폴더에 복사하고 프로젝트 설정 > 플러그인에서 **Fableweld Quests**를 켜세요.
2. Fableweld Quests 도크에서 언어와 퀘스트 프리셋을 고른 뒤 **프리셋 퀘스트 추가**을 누르세요. 선택을 바꾸기 전에 미적용 입력을 적용하거나 되돌리세요.
3. 퀘스트와 목표를 편집하고 **퀘스트 적용**을 누르세요. `res://game_data`와 `res://gameplay`를 만드세요. 카탈로그 경로를 `res://game_data/quests.tres`로 정하고 **저장**을 누르세요.
4. `res://gameplay/quest_playground.tscn` 같은 새 경로를 고르세요. **플레이 예제 만들기**을 누르고 새 장면을 열어 F6으로 실행하세요. 기존 장면 파일은 보존됩니다.
5. 해당 목표를 진행하기 전에 퀘스트를 수락하세요. 시뮬레이션 버튼은 개발 도구입니다. 전투를 시험하려면 호환되는 의존 구성 요소를 설치하고 **연결된 전투 예제 만들기**을 사용하세요. 정원 순찰을 수락하고 적 턴을 진행한 뒤 승리 후 경험치를 받으세요.
6. 언어를 바꾼 뒤 진행을 저장하고 복원하세요. 기본 장면은 퀘스트와 설정된 캐릭터를, 전투 예제는 전투도 저장합니다. 다른 월드 상태는 포함되지 않습니다. 독립된 진행에는 다른 저장 슬롯을 쓰세요.

직접 경험치를 주려면 보상을 설정하고 보상 이벤트를 비운 뒤 퀘스트를 적용하고 생성하세요. 완료 후 한 번 받을 수 있습니다. 생성된 카탈로그와 프로필은 복사본이므로 이후 도크 수정은 기존 장면에 자동 반영되지 않습니다.

업데이트 전에 게임을 멈추고 플러그인을 끈 뒤 편집기를 닫으세요. `addons/fableweld_quests`만 교체하고 UID, 제작 리소스, 장면, 저장 파일을 보존하세요. 복사본에서 시험하세요. ID나 내용 변경으로 이전 저장을 불러오지 못할 수 있으며 자동 이전은 보장되지 않습니다.

현재 서로 호환되는 후보 아카이브를 사용하세요. 이전 검토 ZIP은 이 안내보다 오래되었습니다. [선택적 종속성](DEPENDENCIES.md)을 확인하세요. 공개 배포는 승인되지 않았습니다.

<a id="zh_tw"></a>

## 繁體中文

本版本請使用另外提供的 Fableweld 修正版 Godot 4.7.2。未修改的 4.7.2 可能在結束時當機。請參閱[引擎適用範圍](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md)；本版本另外提供可攜式編輯器。

選用 Inventory 1.0：選擇 **準備背包相容設定**，檢查並確認，然後儲存、關閉並重新開啟專案，再產生背包範例。請將 `res://fableweld_compatibility/inventory-1.0.0/` 與專案備份一起保留。修改過或不受支援的提供方檔案將被拒絕。

1. 先備份 Godot 專案。將 `addons/fableweld_quests` 複製到專案的 `addons` 資料夾，在專案設定 > 外掛中啟用 **Fableweld Quests**。
2. 在 Fableweld Quests 面板中選擇語言和任務預設，按下 **新增預設任務**。切換選擇前，先套用或還原尚未提交的欄位。
3. 編輯任務和目標，按下 **套用任務**。建立 `res://game_data` 和 `res://gameplay` 資料夾。將目錄路徑設為 `res://game_data/quests.tres`，按下 **儲存**。
4. 選擇新的場景路徑，例如 `res://gameplay/quest_playground.tscn`。按下 **建立試玩範例**，開啟新場景並按 F6 執行。既有場景檔案會保留。
5. 先接受任務，再推進對應目標。模擬按鈕僅供開發測試。要體驗戰鬥，請安裝相符的戰鬥相依元件並使用 **建立連接戰鬥範例**；接受花園巡邏，執行敵方回合，獲勝後領取經驗。
6. 使用語言選擇器，然後儲存和還原進度。一般場景儲存任務及已設定角色；戰鬥範例還會儲存戰鬥。其他世界狀態不包含在內。獨立進度請使用不同存檔槽。

若要直接獎勵經驗，請設定任務經驗獎勵，將獎勵事件留空，套用任務後再產生場景。完成後領取一次。產生的目錄和設定是副本；之後的面板修改不會自動更新既有場景。

更新前停止遊戲、停用外掛並關閉編輯器。只替換 `addons/fableweld_quests`，保留腳本 UID、創作資源、場景和存檔。先在備份副本測試。修改 ID 或內容可能導致舊存檔被拒絕；不保證自動遷移。

請使用目前相互配套的候選安裝包。歷史審閱 ZIP 早於本指南。請參閱[選用相依項目](DEPENDENCIES.md)。尚未授權公開發布。

<a id="tr"></a>

## Türkçe

Bu sürüm için ayrı sağlanan Fableweld düzeltmeli Godot 4.7.2 derlemesini kullanın. Değiştirilmemiş 4.7.2 kapanış sırasında çökebilir. [Motor kapsamına](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md) bakın; taşınabilir düzenleyici bu sürüm için ayrı sağlanır.

İsteğe bağlı Inventory 1.0: **Envanter uyumluluğunu hazırla** seçeneğini seçin, inceleyip onaylayın; örneği oluşturmadan önce projeyi kaydedin, kapatıp yeniden açın. `res://fableweld_compatibility/inventory-1.0.0/` dosyalarını proje yedeğiyle saklayın. Değiştirilmiş veya desteklenmeyen sağlayıcı dosyaları reddedilir.

1. Godot projesini yedekleyin. `addons/fableweld_quests` klasörünü projenin `addons` klasörüne kopyalayın. Proje Ayarları > Eklentiler bölümünde **Fableweld Quests** eklentisini etkinleştirin.
2. Fableweld Quests panelinde dili ve görev önayarını seçip **Ön ayar görevi ekle** düğmesine basın. Seçimi değiştirmeden önce bekleyen alanları uygulayın veya geri alın.
3. Görevi ve hedefi düzenleyip **Görevi uygula** düğmesine basın. `res://game_data` ve `res://gameplay` klasörlerini oluşturun. Katalog için `res://game_data/quests.tres` yolunu seçip **Kaydet** düğmesine basın.
4. `res://gameplay/quest_playground.tscn` gibi yeni bir sahne yolu seçin. **Oynanabilir örnek oluştur** düğmesine basın, sahneyi açıp F6 ile çalıştırın. Var olan sahne dosyaları korunur.
5. Eşleşen hedefleri ilerletmeden önce görevi kabul edin. Simülasyon düğmeleri geliştirme araçlarıdır. Savaş için uyumlu bağımlılığı kurup **Bağlı savaş örneği oluştur** düğmesini kullanın; Bahçe devriyesini kabul edin, düşman turlarını yürütün ve zaferden sonra deneyimi alın.
6. Dili değiştirin, ilerlemeyi kaydedip yükleyin. Normal sahne görevleri ve yapılandırılmış karakteri; savaş örneği ayrıca savaşı kaydeder. Diğer dünya durumu kapsam dışıdır. Bağımsız ilerleme için farklı bir kayıt yuvası kullanın.

Doğrudan deneyim için ödülü ayarlayın, ödül olayını boş bırakın ve sahneyi oluşturmadan görevi uygulayın. Tamamlayıp bir kez alın. Oluşturulan katalog ve profiller kopyadır; sonraki panel değişiklikleri mevcut sahneyi güncellemez.

Güncellemeden önce oyunu durdurun, eklentiyi kapatıp düzenleyiciyi kapatın. Yalnızca `addons/fableweld_quests` klasörünü değiştirin; UID, kendi kaynaklarınız, sahneleriniz ve kayıtlarınızı koruyun. Bir kopyada deneyin. ID veya içerik değişiklikleri eski kayıtları reddedebilir; otomatik geçiş sözü verilmez.

Mevcut birbiriyle uyumlu aday arşivleri kullanın. Eski inceleme ZIP dosyası bu kılavuzdan öncedir. [İsteğe bağlı bağımlılıklar](DEPENDENCIES.md) bölümüne bakın. Yayımlama yetkisi verilmemiştir.

<a id="uk"></a>

## Українська

Для цього випуску використовуйте окремо надану виправлену збірку Godot 4.7.2 від Fableweld. Незмінена версія 4.7.2 може аварійно завершитися під час закриття. Див. [межі підтримки рушія](https://github.com/fableweldlabs/fableweldlabs/blob/main/QUESTS-ENGINE-SCOPE.md); портативний редактор надається окремо для цього випуску.

Додаткова Inventory 1.0: виберіть **Підготувати сумісність інвентарю**, перевірте й підтвердьте, а потім збережіть, закрийте та знову відкрийте проєкт перед створенням прикладу. Зберігайте `res://fableweld_compatibility/inventory-1.0.0/` разом із резервною копією проєкту. Змінені або непідтримувані файли постачальника відхиляються.

1. Зробіть резервну копію проєкту Godot. Скопіюйте `addons/fableweld_quests` до його папки `addons`. Увімкніть **Fableweld Quests** у налаштуваннях проєкту > Додатки.
2. У панелі Fableweld Quests виберіть мову й шаблон завдання, потім натисніть **Додати шаблонне завдання**. Перш ніж змінювати вибір, застосуйте або скасуйте незастосовані поля.
3. Відредагуйте завдання й ціль та натисніть **Застосувати завдання**. Створіть `res://game_data` і `res://gameplay`. Виберіть `res://game_data/quests.tres` для каталогу та натисніть **Зберегти**.
4. Виберіть новий шлях, наприклад `res://gameplay/quest_playground.tscn`. Натисніть **Створити ігровий приклад**, відкрийте сцену й запустіть її клавішею F6. Наявні файли сцен зберігаються.
5. Прийміть завдання перед виконанням відповідних цілей. Кнопки симуляції призначені для розробки. Для бою встановіть сумісну залежність і скористайтеся **Створити пов’язаний приклад бою**; прийміть Патруль саду, виконуйте ходи ворога й отримайте досвід після перемоги.
6. Змініть мову, збережіть і відновіть поступ. Звичайна сцена зберігає завдання й налаштованого персонажа; бойовий приклад також зберігає бій. Інший стан світу не входить до запису. Для незалежного поступу використовуйте інший слот.

Для прямого досвіду задайте нагороду, залиште подію нагороди порожньою та застосуйте завдання до створення сцени. Завершіть і отримайте нагороду один раз. Створені каталоги й профілі є копіями; подальші зміни панелі не оновлюють наявну сцену.

Перед оновленням зупиніть гру, вимкніть додаток і закрийте редактор. Замініть лише `addons/fableweld_quests`; збережіть UID, власні ресурси, сцени та записи гри. Перевіряйте в копії. Зміни ID чи вмісту можуть спричинити відмову старого запису; автоматичне перенесення не обіцяється.

Використовуйте поточні узгоджені архіви кандидатів. Історичний ZIP для перевірки старіший за цей посібник. Див. [Необов’язкові залежності](DEPENDENCIES.md). Публікацію не дозволено.


## Appearance and navigation (en)

Choose Light for a bright workspace or Dark for a dim workspace. Fableweld and Gold are optional styles. Your choice is remembered separately from game saves.

Use 100%, 125% or 150% text size. Find action searches the currently available buttons. Select a result to move keyboard focus to it; the action is not executed. Press Escape to close the search.

Changing appearance does not translate your authored names or change your game language. Existing features and save formats remain available.

## Apariencia y navegación (es)

Elige Claro para un entorno luminoso u Oscuro para uno con poca luz. Fableweld y Dorado son estilos opcionales. La elección se guarda por separado de las partidas.

Elige un tamaño de texto del 100 %, 125 % o 150 %. Buscar acción busca entre los botones disponibles. Selecciona un resultado para mover el foco del teclado sin ejecutar la acción. Pulsa Esc para cerrar la búsqueda.

Cambiar la apariencia no traduce los nombres creados por ti ni cambia el idioma del juego. Se mantienen las funciones y los formatos de guardado existentes.

## Aparência e navegação (pt_BR)

Escolha Claro para um ambiente iluminado ou Escuro para um ambiente com pouca luz. Fableweld e Dourado são estilos opcionais. A escolha é salva separadamente dos jogos salvos.

Escolha o tamanho de texto de 100%, 125% ou 150%. Buscar ação pesquisa os botões disponíveis. Selecione um resultado para mover o foco do teclado sem executar a ação. Pressione Esc para fechar a busca.

Alterar a aparência não traduz os nomes que você criou nem muda o idioma do jogo. Os recursos e formatos de salvamento existentes são mantidos.

## 外观与导航 (zh_CN)

明亮环境可选择浅色主题，昏暗环境可选择深色主题。也可选用 Fableweld 或金色主题。外观偏好与游戏存档分开保存。

文字大小可设为 100%、125% 或 150%。查找操作会搜索当前可用的按钮。选择结果只会将键盘焦点移到对应按钮，不会执行操作。按 Esc 关闭搜索。

更改外观不会翻译您创作的名称，也不会改变游戏语言。现有功能和存档格式保持兼容。

## 外観と操作 (ja)

明るい環境ではライト、暗い環境ではダークを選べます。Fableweld とゴールドも利用できます。外観設定はゲームのセーブデータとは別に保存されます。

文字サイズは 100%、125%、150% から選べます。「操作を探す」で現在利用できるボタンを検索できます。結果を選ぶとキーボードのフォーカスが移動しますが、操作は実行されません。Esc キーで検索を閉じます。

外観を変更しても、作成した名前の翻訳やゲーム言語の変更は行われません。既存の機能とセーブ形式は引き続き利用できます。

## Apparence et navigation (fr)

Choisissez Clair dans un environnement lumineux ou Sombre dans un environnement peu éclairé. Fableweld et Or sont des styles facultatifs. Ce choix est enregistré séparément des sauvegardes du jeu.

Choisissez une taille de texte de 100 %, 125 % ou 150 %. Trouver une action recherche les boutons disponibles. Sélectionner un résultat déplace le focus clavier sans exécuter l’action. Appuyez sur Échap pour fermer la recherche.

Changer l’apparence ne traduit pas les noms que vous avez créés et ne change pas la langue du jeu. Les fonctions et formats de sauvegarde existants restent disponibles.

## Darstellung und Navigation (de)

Wähle Hell für eine helle Arbeitsumgebung oder Dunkel für eine dunkle Umgebung. Fableweld und Gold stehen zusätzlich zur Wahl. Die Einstellung wird getrennt von Spielständen gespeichert.

Wähle 100 %, 125 % oder 150 % Textgröße. Aktion finden durchsucht die verfügbaren Schaltflächen. Ein Suchergebnis verschiebt den Tastaturfokus, ohne die Aktion auszuführen. Mit Esc schließt du die Suche.

Ein Darstellungswechsel übersetzt keine selbst vergebenen Namen und ändert nicht die Spielsprache. Bestehende Funktionen und Speicherformate bleiben erhalten.

## Wygląd i nawigacja (pl)

Wybierz jasny motyw w jasnym otoczeniu lub ciemny przy słabym oświetleniu. Fableweld i Złoty to dodatkowe style. Ustawienie jest zapisywane osobno od zapisów gry.

Wybierz rozmiar tekstu 100%, 125% lub 150%. Znajdź działanie przeszukuje dostępne przyciski. Wybranie wyniku przenosi fokus klawiatury, ale nie wykonuje działania. Naciśnij Esc, aby zamknąć wyszukiwanie.

Zmiana wyglądu nie tłumaczy utworzonych przez Ciebie nazw ani nie zmienia języka gry. Dotychczasowe funkcje i formaty zapisów pozostają dostępne.

## 모양 및 탐색 (ko)

밝은 환경에서는 라이트 테마를, 어두운 환경에서는 다크 테마를 선택하세요. Fableweld와 골드 테마도 사용할 수 있습니다. 모양 설정은 게임 저장 데이터와 별도로 저장됩니다.

글자 크기는 100%, 125%, 150% 중에서 선택할 수 있습니다. 동작 찾기는 현재 사용 가능한 버튼을 검색합니다. 검색 결과를 선택하면 키보드 초점만 이동하며 동작은 실행되지 않습니다. Esc 키를 누르면 검색이 닫힙니다.

모양을 변경해도 직접 작성한 이름을 번역하거나 게임 언어를 바꾸지 않습니다. 기존 기능과 저장 형식은 계속 사용할 수 있습니다.

## 外觀與導覽 (zh_TW)

明亮環境可選擇淺色主題，昏暗環境可選擇深色主題。也可選用 Fableweld 或金色主題。外觀偏好與遊戲存檔分開儲存。

文字大小可設為 100%、125% 或 150%。尋找操作會搜尋目前可用的按鈕。選擇結果只會將鍵盤焦點移到對應按鈕，不會執行操作。按 Esc 關閉搜尋。

變更外觀不會翻譯您創作的名稱，也不會改變遊戲語言。現有功能和存檔格式保持相容。

## Görünüm ve gezinme (tr)

Aydınlık ortamlarda Açık, loş ortamlarda Koyu temayı seçin. Fableweld ve Altın isteğe bağlı stillerdir. Seçiminiz oyun kayıtlarından ayrı saklanır.

Metin boyutunu %100, %125 veya %150 olarak seçin. Eylem bul, kullanılabilir düğmeler arasında arama yapar. Bir sonucu seçmek klavye odağını taşır; eylemi çalıştırmaz. Aramayı kapatmak için Esc tuşuna basın.

Görünümü değiştirmek oluşturduğunuz adları çevirmez ve oyunun dilini değiştirmez. Mevcut özellikler ve kayıt biçimleri korunur.

## Вигляд і навігація (uk)

Виберіть світлу тему для яскравого оточення або темну для слабкого освітлення. Fableweld і Золота є додатковими стилями. Налаштування зберігається окремо від збережень гри.

Виберіть розмір тексту 100%, 125% або 150%. Знайти дію виконує пошук серед доступних кнопок. Вибір результату лише переміщує фокус клавіатури й не виконує дію. Натисніть Esc, щоб закрити пошук.

Зміна вигляду не перекладає створені вами назви й не змінює мову гри. Наявні функції та формати збережень залишаються доступними.
