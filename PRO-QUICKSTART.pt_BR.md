Calendar & Growth Pro — Guia rápido
Documentação da versão candidata 2.1.0; ainda não publicada.

1. Copie addons/rpg_time para seu projeto. Ative o complemento em Project > Project Settings > Plugins. Para testar o exemplo, extraia a descarga separadamente e abra o project.godot dela; não substitua o arquivo do seu jogo.
2. Abra Time & Seasons e escolha Português (Brasil) em Language. O idioma do painel não muda o idioma do Godot nem o do jogo.
3. Em Configuração, escolha um caminho res:// fora de addons e clique em Salvar perfil. Os campos só entram em vigor ao clicar em Aplicar. Aplique ou reverta antes de mudar de seção.
4. Em Calendário, configure meses, dias e estações. Nomes personalizados são salvos exatamente como digitados. Em Períodos, o primeiro começa às 00:00; os demais devem estar em ordem.
5. Para crescimento, escolha uma predefinição e ajuste o ritmo. Depois, edite a maturidade e as etapas individualmente. Mover o controle ou escolher outra predefinição substitui essas edições. Os valores se aplicam à próxima cena gerada.
6. Salve o perfil e gere a estrutura desejada. Arraste a cena para o mundo ou use a inserção do painel. Mantenha um único relógio principal; não adicione outro CanvasModulate a um canvas já conectado.
7. Use Prévia para testar tempo, estações e eventos sem alterar o relógio do jogo ou os salvamentos. Saltos que atravessem mais de 10.000 eventos são rejeitados.

Os controles reutilizáveis têm interface_language no Inspector. Após alterar durante o jogo, chame refresh(). Títulos, nomes e mensagens personalizados continuam sob seu controle para tradução. Deixe vazio o texto do botão de dormir para usar a legenda traduzida automática.

save_file/load_file salvam o relógio, não um jogo completo. Preserve os salvamentos originais ao testar atualizações. Alterar definições de calendário ou eventos pode exigir migração. Perfis opcionais de atmosfera ampliam a iluminação básica; não inclui clima, combate ou movimento de NPC.


Atmosfera e ferramentas de desenvolvimento
Em Iluminação, escolha e aplique uma predefinição de atmosfera. Os interruptores preservam as curvas editadas manualmente. Salve o perfil e gere uma nova configuração. No exemplo opcional Lumen Vale, abra Calendário e role até Atmosfera. Sem atmosfera mantém o visual original. A prévia e o interruptor de neblina não alteram o perfil salvo; remover a prévia restaura a iluminação original.

As ferramentas locais de desenvolvimento são incluídas apenas quando selecionadas na geração. Estão desativadas por padrão, conectam-se automaticamente ao relógio e permanecem desativadas no executável de lançamento. DEVELOPMENT-BRIDGE.md descreve o contrato Fableweld; nenhum acesso à rede é aberto.
