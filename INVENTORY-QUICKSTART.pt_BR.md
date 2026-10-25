# Inventário e equipamentos — início rápido

Inventário e equipamento 1.0.0. Godot 4.7.2, Windows x64. Consulte a licença e os avisos dos componentes incluídos.

1. Preserve uma cópia do projeto e dos salvamentos. Copie
   `addons/fableweld_inventory` para o jogo. Compare versões e preserve suas
   alterações antes de substituir arquivos. Não exige relógio nem addon de NPCs.
2. Ative Fableweld Inventory & Equipment em Configurações do Projeto > Plugins.
   Escolha o idioma do painel. Isso não altera a localidade global do jogo.
3. Crie itens ou adicione itens iniciais. Edite no Inspetor e valide o catálogo.
   Salve um `.tres` fora de `addons`. Carregue um destino existente antes de
   atualizá-lo; o carregamento exige confirmação. Mantenha os IDs estáveis.
4. No projeto de exemplo, abra `demo/inventory_quick_start.tscn` e pressione F6.
   O seletor superior coordena abas e painéis. Equipe a lâmina inicial, atribua
   uma poção à barra de atalhos, divida uma pilha e transfira para o baú.
5. Nas suas cenas, aponte `controller_path` dos painéis para um
   `FWSlotInventoryController`. Grades que trocam itens precisam do mesmo recurso
   de catálogo e de um `transfer_group` não vazio. Seu jogo fornece os efeitos
   dos itens e os atributos básicos.
6. Registre controladores em `FWInventorySession.controllers` com IDs estáveis de
   salvamento e NodePaths. Aponte `FWInventorySavePanel.session_path` para essa
   sessão. Escolha um `user://...json` diferente para cada espaço de salvamento
   ou mundo.
7. Salve e carregue a sessão de inventário. Ela inclui bolsas registradas,
   equipamentos e atalhos; não salva o jogo inteiro. O exemplo antigo perde o
   ponto de controle ao fechar. Preserve qualquer `.fw-writing` existente antes
   de repetir um salvamento bloqueado. Escritas simultâneas não são suportadas.
8. Atualize primeiro uma cópia. Mantenha catálogos, cenas e salvamentos fora das
   pastas do fornecedor. Para remover, substitua referências dependentes,
   desative o plugin e remova a pasta do addon. Apagar scripts ainda
   referenciados quebra as cenas.

Trocar o idioma preserva IDs e textos personalizados. A tradução das categorias
e atributos do exemplo é opcional via `translate_example_names`, desativada por
padrão nas interfaces reutilizáveis. Textos personalizados desconhecidos são
preservados. Não se afirma revisão por falantes nativos, compatibilidade com
qualquer projeto ou aceitação final dos pacotes exportados.
