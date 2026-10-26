# RPG Combat for Godot

[Official product and downloads](https://fableweld-labs.itch.io/rpg-combat) · [Bug reports](https://github.com/fableweldlabs/fableweldlabs/issues)

Turn-based battles, abilities, statuses, party progression, enemy decisions and editable difficulty tiers. Built-in UI and guides support English, Spanish, Brazilian Portuguese, Simplified Chinese, Japanese, French and German, with English fallback. Translations are AI-assisted.

Only the small addon is required. The editable example and free Windows demo are separate optional downloads. Reusable controls are 2D; the optional Lumen Vale world is 3D. Combat works standalone; Characters is optional and sold separately.

## Capabilities

- Initiative, legal targets, costs, accuracy, damage/healing, Guard, Pass and results.
- Shared-duration status stacks, stat modifiers, action restrictions and turn-end HP effects.
- Enemy legal-action selection and healing thresholds.
- Party recruitment, roster, growth, XP and one-time rewards.
- Difficulty recommendations with pinned manual values, preview, explicit apply/undo, tier CRUD and removed-tier migration.
- Validated resource catalogs, editor session history, reusable battle and roster controls.
- Battle/party snapshots and RNG persistence. The optional campaign shows carried wounds, rest, three slots and backup recovery.

## Requirements and limits

Verified on Godot 4.7.2 Windows x64. Other platforms are unverified. Your game coordinates enemy scheduling, encounters, items, economy, quests and whole-game storage. Examples show integration. Reference difficulty settings require tuning for your authored enemies, gear and campaign. This is not a real-time or tactical-grid combat system, skill-tree editor or complete RPG authoring kit.

Validation includes automated native workflows and reviewed captures. It does not establish human normal-play, native-speaker, physical-DPI or complete accessibility certification. Narrow long editor labels may be ellipsized; custom content needs host layout review. Dock history covers creation/replacement snapshots within a session, not general Inspector undo.

## Licensing and support

Copyright 2026 Gordon Hinchen; Fableweld Labs branding. Paid addon source remains private. One purchasing person/entity and its private project team may use the commercial additions in unlimited integrated games/apps under the included commercial license. Separately licensed components retain their own rights. Read LICENSE.md, LICENSE-COMPONENTS.txt and notices. Refunds follow itch.io processes and mandatory rights.

Email fableweldlabs@gmail.com or open an issue with engine/product version, reproduction steps and safe screenshots. Keep paid source and private saves out of public reports.

# Combat quick starts

Development documentation. Exact customer packages and native acceptance remain pending. These guides describe the current source; independent native-speaker review has not been performed. See [installation and updates](INSTALLATION.md) and the [API reference](README.md).

## Difficulty workflow / Flujo de dificultad / Fluxo de dificuldade / 难度流程 / 難易度の手順 / Réglage de difficulté / Schwierigkeitsablauf

**English:** Open the difficulty workspace from the Combat dock. Create or load a tier, choose a style and preview recommendations. Manual edits remain fixed until you release that field to automatic values. Compare before/after, apply explicitly, then save the catalog in the dock. Undo restores the previous applied tier when it has not changed elsewhere. Duplicate tiers to compare alternatives. Renaming keeps the ID; removal requires a replacement or authored defaults for old saves. In the campaign, choose a tier before starting battle. Levels and earned XP are retained; switching during battle is unavailable. Recommendations and the reference duel do not guarantee balanced encounters.

**Español:** Abre el espacio de dificultad desde el panel Combate. Crea o carga un nivel, elige un estilo y previsualiza las recomendaciones. Los valores manuales se conservan hasta volver a activar el valor automático del campo. Compara el antes y el después, aplica y guarda el catálogo en el panel. Deshacer restaura el nivel anterior si no cambió en otro lugar. Duplica niveles para compararlos. Cambiar el nombre conserva el ID; al eliminar, elige un reemplazo o los valores originales para las partidas antiguas. Elige la dificultad antes del combate. Se conservan los niveles y la experiencia obtenida; no se cambia durante el combate. Las recomendaciones y el duelo de referencia no garantizan encuentros equilibrados.

**Português brasileiro:** Abra o espaço de dificuldade no painel Combate. Crie ou carregue um nível, escolha um estilo e visualize as recomendações. Valores manuais permanecem fixos até você restaurar o valor automático do campo. Compare antes e depois, aplique e salve o catálogo no painel. Desfazer restaura o nível anterior se ele não mudou em outro lugar. Duplique níveis para comparar opções. Renomear mantém o ID; ao remover, escolha um substituto ou os valores originais para os saves antigos. Escolha a dificuldade antes do combate. Níveis e experiência obtida são preservados; não é possível trocar durante o combate. As recomendações e o duelo de referência não garantem encontros equilibrados.

**简体中文：** 从战斗面板打开难度工作区。创建或载入难度档位，选择风格并预览推荐值。手动修改的字段会保持固定，直到将该字段恢复为自动值。比较修改前后，明确应用后再从面板保存目录。若该档位未被其他操作修改，可以撤销上次应用。复制档位可比较不同方案。重命名不会改变 ID；删除时必须为旧存档指定替代档位或原始设定。请在战斗开始前选择难度。等级和已获得的经验会保留，战斗中不能切换。推荐值和参考对决并不保证遭遇战平衡。

**日本語：** 戦闘ドックから難易度ワークスペースを開きます。難易度を作成または読み込み、スタイルを選んで推奨値を確認します。手動で編集した値は、その項目を自動値に戻すまで保持されます。変更前後を比較して適用し、ドックでカタログを保存してください。他の操作で変更されていなければ、直前の適用を元に戻せます。複製して設定を比較できます。名前を変えても ID は変わりません。削除時は古いセーブ用の移行先、または元の設定を選びます。難易度は戦闘前に選択します。レベルと獲得済み経験値は保持され、戦闘中は変更できません。推奨値と参考対決は戦闘バランスを保証しません。

**Français :** Ouvrez l’espace de difficulté depuis le panneau Combat. Créez ou chargez un palier, choisissez un style et prévisualisez les recommandations. Les valeurs manuelles restent fixes jusqu’au rétablissement du mode automatique du champ. Comparez avant et après, appliquez, puis enregistrez le catalogue dans le panneau. Annuler restaure le palier précédent s’il n’a pas été modifié ailleurs. Dupliquez les paliers pour les comparer. Renommer conserve l’identifiant ; supprimer exige un remplacement ou les valeurs d’origine pour les anciennes sauvegardes. Choisissez la difficulté avant le combat. Les niveaux et l’expérience acquise sont conservés ; aucun changement n’est possible pendant le combat. Les recommandations et le duel de référence ne garantissent pas l’équilibre des rencontres.

**Deutsch:** Öffne den Schwierigkeitsbereich im Kampf-Dock. Erstelle oder lade eine Stufe, wähle einen Stil und prüfe die Empfehlungen. Manuell bearbeitete Werte bleiben erhalten, bis du das jeweilige Feld auf automatisch zurücksetzt. Vergleiche vorher und nachher, wende die Änderungen an und speichere den Katalog im Dock. Rückgängig stellt die zuvor angewendete Stufe wieder her, sofern sie nicht anderweitig geändert wurde. Dupliziere Stufen zum Vergleichen. Umbenennen behält die ID bei; beim Löschen wählst du einen Ersatz oder die ursprünglichen Werte für alte Spielstände. Wähle die Schwierigkeit vor dem Kampf. Stufen und verdiente Erfahrung bleiben erhalten; während des Kampfes ist kein Wechsel möglich. Empfehlungen und Referenzduell garantieren keine ausgewogenen Begegnungen.

## English

1. Extract the optional editable example into its own folder. Open `project.godot` with Godot 4.7.2 and wait for import. Run `demo/battle_demo.tscn` for practice. Choose a language from the list.
2. Choose an ability and a legal target, then use the ability. The example handles enemy turns. Guard reduces incoming damage; Pass ends the current turn. Focus increases attack, Venom causes turn-end damage, and Stun forces a pass.
3. Run `examples/campaign_demo.tscn` for a campaign. Select up to two members, apply the party, then start an encounter. Selection changes are drafts until applied.
4. Victories award experience once. New level statistics apply next encounter. Wounds and spent resources carry forward; Rest restores starting vitals for the next encounter. Party changes and rest are unavailable during battle.
5. Choose a slot and save. Load replaces current progress with that slot. If the primary save fails to load, try Load backup and save recovered progress to another slot. Existing recovery files block replacement; keep them until recovery is verified.
6. To author content, enable **Fableweld Combat & Parties** in Project Settings → Plugins. Create a starter catalog in an empty dock, edit entries in the Inspector and save a `.tres` outside `addons`. Keep stable IDs separate from translated display names. The optional world offers Practice Battle and Party Campaign; Close returns to the world.

## Español

1. Extrae el ejemplo editable opcional en su propia carpeta. Abre `project.godot` con Godot 4.7.2 y espera a que termine la importación. Ejecuta `demo/battle_demo.tscn` para practicar. Selecciona el idioma en la lista.
2. Elige una habilidad y un objetivo válido y usa la habilidad. El ejemplo controla los turnos enemigos. Defender reduce el daño recibido; Pasar termina el turno. Concentración aumenta el ataque, Veneno causa daño al finalizar el turno y «Aturdir» obliga a pasar.
3. Ejecuta `examples/campaign_demo.tscn`. Selecciona hasta dos miembros, aplica el grupo e inicia un encuentro. Los cambios de selección no se confirman hasta aplicarlos.
4. Cada victoria concede experiencia una sola vez. Los atributos del nuevo nivel se aplican en el siguiente encuentro. Las heridas y los recursos gastados se conservan; descansar restaura los valores iniciales para el siguiente combate. No puedes descansar ni cambiar el grupo durante el combate.
5. Elige una ranura y guarda. Cargar reemplaza el progreso actual. Si no puedes cargar el archivo principal, prueba Cargar respaldo y guarda lo recuperado en otra ranura. Los archivos de recuperación existentes impiden sobrescribir; consérvalos hasta verificar la recuperación.
6. Para crear contenido, activa **Fableweld Combat & Parties** en Project Settings → Plugins. Crea un catálogo inicial en el panel vacío, edita las entradas en el Inspector y guarda un `.tres` fuera de `addons`. Conserva los identificadores aunque traduzcas los nombres. El mundo opcional ofrece práctica y campaña; Cerrar vuelve al mundo.

## Português (Brasil)

1. Extraia o exemplo editável opcional em uma pasta própria. Abra `project.godot` no Godot 4.7.2 e aguarde a importação. Execute `demo/battle_demo.tscn` para treinar. Escolha o idioma na lista.
2. Escolha uma habilidade e um alvo válido e use a habilidade. O exemplo controla os turnos inimigos. Defender reduz o dano recebido; Passar encerra o turno. Concentração aumenta o ataque, Veneno causa dano no fim do turno e “Atordoar” força a passagem do turno.
3. Execute `examples/campaign_demo.tscn`. Selecione até dois membros, aplique o grupo e inicie um encontro. A seleção só é confirmada ao aplicar.
4. Cada vitória concede experiência uma vez. Os atributos do novo nível valem no próximo encontro. Ferimentos e recursos gastos são mantidos; descansar restaura os valores iniciais para o próximo combate. Não é possível descansar nem mudar o grupo durante a batalha.
5. Escolha um espaço e salve. Carregar substitui o progresso atual. Se o arquivo principal não carregar, tente Carregar backup e salve o progresso recuperado em outro espaço. Arquivos de recuperação existentes impedem a substituição; preserve-os até verificar a recuperação.
6. Para criar conteúdo, ative **Fableweld Combat & Parties** em Project Settings → Plugins. Crie um catálogo inicial no painel vazio, edite as entradas no Inspector e salve um `.tres` fora de `addons`. Mantenha os IDs estáveis ao traduzir os nomes. O mundo opcional oferece treino e campanha; Fechar retorna ao mundo.

## 简体中文

1. 将可选的可编辑示例解压到单独的文件夹。使用 Godot 4.7.2 打开 `project.godot`，等待导入完成。运行 `demo/battle_demo.tscn` 进行练习，并从列表中选择语言。
2. 选择技能和有效目标，然后使用技能。示例会处理敌方回合。防御可减少受到的伤害；跳过会结束当前回合。专注提高攻击力，毒素在回合结束时造成伤害，眩晕迫使目标跳过行动。
3. 运行 `examples/campaign_demo.tscn` 开始战役。最多选择两名成员，应用队伍后开始遭遇战。应用前的选择只是草稿。
4. 每场胜利只发放一次经验值。升级后的属性在下一场战斗生效。伤势和资源消耗会保留；休息可让下一场战斗使用初始生命和资源。战斗期间不能休息或更换队伍。
5. 选择存档位并保存。加载会替换当前进度。如果主存档无法加载，请尝试加载备份，再将恢复的进度保存到其他存档位。已有恢复文件时不能覆盖；确认恢复成功前请保留这些文件。
6. 要制作内容，请在 Project Settings → Plugins 中启用 **Fableweld Combat & Parties**。在空面板中创建初始目录，用 Inspector 编辑条目，并将 `.tres` 保存到 `addons` 以外。翻译显示名称时保持 ID 不变。可选世界提供练习战斗和队伍战役；关闭面板可返回世界。

## 日本語

1. 任意の編集可能サンプルを専用フォルダーに展開します。Godot 4.7.2 で `project.godot` を開き、インポート完了を待ちます。練習には `demo/battle_demo.tscn` を実行し、一覧から言語を選びます。
2. アビリティと有効な対象を選び、実行します。敵のターンはサンプルが処理します。防御は被ダメージを減らし、パスは現在のターンを終了します。集中は攻撃力を上げ、毒はターン終了時にダメージを与え、気絶は行動をパスさせます。
3. キャンペーンには `examples/campaign_demo.tscn` を実行します。最大2人を選び、パーティーを適用してから戦闘を開始します。適用するまで選択は未確定です。
4. 勝利の経験値は各戦闘につき一度だけ加算されます。レベルアップ後の能力値は次の戦闘で反映されます。傷と消費したリソースは持ち越されます。休息すると次の戦闘は初期の生命力とリソースで始まります。戦闘中は休息や編成変更ができません。
5. スロットを選んで保存します。読み込みは現在の進行状況を置き換えます。通常のセーブを読めない場合はバックアップを読み込み、復旧した進行を別スロットに保存してください。復旧用ファイルがあると上書きできません。復旧を確認するまで保持してください。
6. 制作には Project Settings → Plugins で **Fableweld Combat & Parties** を有効にします。空のドックで初期カタログを作り、Inspector で項目を編集し、`.tres` を `addons` の外に保存します。表示名を翻訳しても ID は変えません。任意のワールドには練習とキャンペーンがあり、閉じるとワールドに戻ります。

## Français

1. Extrayez l’exemple modifiable facultatif dans son propre dossier. Ouvrez `project.godot` avec Godot 4.7.2 et attendez la fin de l’importation. Lancez `demo/battle_demo.tscn` pour vous entraîner. Choisissez une langue dans la liste.
2. Choisissez une compétence et une cible valide, puis utilisez la compétence. L’exemple gère les tours ennemis. Se défendre réduit les dégâts reçus ; Passer termine le tour. Concentration augmente l’attaque, Venin inflige des dégâts en fin de tour et « Étourdir » force à passer.
3. Lancez `examples/campaign_demo.tscn`. Sélectionnez au maximum deux membres, appliquez l’équipe, puis commencez un combat. La sélection reste provisoire jusqu’à son application.
4. Chaque victoire rapporte de l’expérience une seule fois. Les nouvelles statistiques s’appliquent au combat suivant. Blessures et ressources dépensées sont conservées ; le repos rétablit les valeurs initiales pour le prochain combat. Le repos et les changements d’équipe sont indisponibles pendant le combat.
5. Choisissez un emplacement et sauvegardez. Charger remplace la progression actuelle. Si le fichier principal ne se charge pas, essayez la sauvegarde de secours, puis sauvegardez la progression récupérée dans un autre emplacement. Les fichiers de récupération existants empêchent le remplacement ; conservez-les jusqu’à vérification.
6. Pour créer du contenu, activez **Fableweld Combat & Parties** dans Project Settings → Plugins. Créez un catalogue initial dans le panneau vide, modifiez les entrées dans l’Inspector et enregistrez un `.tres` hors de `addons`. Gardez les identifiants stables lorsque vous traduisez les noms. Le monde facultatif propose entraînement et campagne ; Fermer revient au monde.

## Deutsch

1. Entpacke das optionale bearbeitbare Beispiel in einen eigenen Ordner. Öffne `project.godot` mit Godot 4.7.2 und warte auf den Import. Starte `demo/battle_demo.tscn` zum Üben. Wähle eine Sprache aus der Liste.
2. Wähle eine Fähigkeit und ein gültiges Ziel und setze die Fähigkeit ein. Das Beispiel übernimmt die Gegnerzüge. Verteidigen verringert eingehenden Schaden; Passen beendet den Zug. Fokus erhöht den Angriff, Gift verursacht Schaden am Zugende und „Betäuben“ erzwingt das Passen.
3. Starte `examples/campaign_demo.tscn`. Wähle höchstens zwei Mitglieder, übernimm die Gruppe und beginne einen Kampf. Die Auswahl bleibt bis zur Übernahme ein Entwurf.
4. Jeder Sieg vergibt einmal Erfahrung. Neue Stufenwerte gelten ab dem nächsten Kampf. Wunden und verbrauchte Ressourcen bleiben erhalten; Ausruhen stellt die Anfangswerte für den nächsten Kampf wieder her. Während des Kampfes sind Ruhe und Gruppenwechsel gesperrt.
5. Wähle einen Speicherplatz und speichere. Laden ersetzt den aktuellen Fortschritt. Falls der Hauptspielstand nicht geladen werden kann, lade die Sicherung und speichere den wiederhergestellten Fortschritt auf einem anderen Platz. Vorhandene Wiederherstellungsdateien verhindern das Überschreiben; bewahre sie bis zur bestätigten Wiederherstellung auf.
6. Aktiviere zum Erstellen von Inhalten **Fableweld Combat & Parties** unter Project Settings → Plugins. Erstelle im leeren Dock einen Startkatalog, bearbeite Einträge im Inspector und speichere eine `.tres` außerhalb von `addons`. Übersetze Anzeigenamen, ohne stabile IDs zu ändern. Die optionale Welt bietet Übung und Kampagne; Schließen führt zur Welt zurück.
