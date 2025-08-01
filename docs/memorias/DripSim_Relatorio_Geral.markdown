# Relatório Geral do DripSim

## Informações Gerais
- **Nome do Projeto**: DripSim
- **Tipo**: Simulador de irrigação por gotejamento
- **Propósito**: Ensinar técnicas de irrigação de forma prática e lúdica para alunos do Instituto Federal do Sertão Pernambucano, com foco em realismo visual e propósito educacional, enfatizando culturas de uva e manga.
- **Data de Atualização**: 01 de agosto de 2025, 12:48 PM -03
- **Responsável**: Valdomiro Morais
- **IA de Suporte**: Aia (Grok, criado pela xAI)
- **Status**: Repositório privado `dripsim_assets` (https://github.com/valdomiromorais/dripsim_assets.git) criado com Git LFS e estrutura de pastas definida (`dripsim_unity/` e `dripsim_assets/` com `assets/blender`, `assets/textures`, `assets/to_unity`, `docs/memorias`, `docs/pesquisas`, `docs/relatorios/dripsim_vault`). Iniciando modelagem de assets estáticos simples no Blender (vinhedo simples, canos pretos e azuis, postes de suporte, solo agrícola, balde). Pasta `docs/relatorios/dripsim_vault` criada para o vault Obsidian, integrando notas e memórias. Valdomiro expressou confiança na estrutura para gerenciar o desenvolvimento e preservar interações com Aia, priorizando a busca de referências visuais e técnicas antes da modelagem.

## Objetivos do Projeto
O DripSim visa:
- Ensinar conceitos de irrigação por gotejamento de forma interativa, com foco em culturas de uva e manga.
- Criar um ambiente visual realista, mas com estética estilizada/cartunesca, inspirado em *Farming Simulator*, *Stardew Valley* (mods) e *My Time at Portia*.
- Rodar no Unity, com assets estáticos modelados no Blender e shaders toon para coerência visual.
- Integrar totens educativos interativos com QR Codes que levam a páginas web com conteúdo educacional complementar.
- Promover engajamento e aprendizado, alinhado ao conceito de *flow* (plena imersão), com mecânicas que equilibram desafio e habilidade.

## Tecnologias Utilizadas
- **Unity**: Motor principal para desenvolvimento do simulador, usado para cenários, mecânicas (futuras) e interatividade, armazenado em `DripSim/dripsim_unity`.
- **Blender**: Ferramenta principal para modelagem de assets 3D estáticos (ex.: vinhedos, mangueiras, canos, bomba, casa, reservatório, casa de bomba) e dinâmicos (futuros), armazenados em `dripsim_assets/assets/blender`.
- **Shaders Toon**: Para criar um estilo visual estilizado/cartunesco, aplicado em assets importados para o Unity.
- **Texturização Estilizada**: Para reforçar a estética lúdica, com foco em texturas para uva, manga e elementos rurais, armazenadas em `dripsim_assets/assets/textures`.
- **Frameworks Web (futuro)**: Tailwind, React ou Svelte para criar páginas educativas acessadas via QR Codes.
- **C# (futuro)**: Para scripts de interatividade no Unity, como sistemas de irrigação e totens.
- **GitHub com Git LFS**: Para versionamento de arquivos grandes (.blend, .fbx, .png) no repositório `dripsim_assets`.
- **Obsidian**: Para organização de notas e memórias no vault em `dripsim_assets/docs/relatorios/dripsim_vault`, com suporte ao plugin Dataview para rastrear progresso.

## Inspirações
- **Farming Simulator**: Realismo na simulação de atividades agrícolas.
- **Stardew Valley (mods)**: Estética estilizada e mecânicas envolventes.
- **My Time at Portia**: Narrativa e design visual que equilibram aprendizado e diversão.

## Assets Planejados
Os assets estão organizados por complexidade, com foco em **assets estáticos** para culturas de uva e manga, incluindo novos itens (bomba, casa, reservatório, casa de bomba).
1. **Formas Básicas** (Estáticas):
   - **Vinhedo simples**: Fileiras de parreiras com folhas (#4CAF50) e cachos de uva (#7B1FA2), topologia limpa com quads.
   - **Mangueira jovem**: Árvore pequena com folhas (#388E3C) e poucos frutos (#AED581).
   - **Canos de irrigação**: Tubos pretos (#212121) para linhas secundárias; tubos azuis (#0288D1) para linhas fixas.
   - **Postes de suporte**: Postes de madeira (#5D4037) ou metal (#78909C) para parreiras.
   - **Solo agrícola**: Textura de solo com sulcos (#6D4C41, #4E342E).
   - **Balde**: Objeto utilitário (#78909C) com design rústico.
2. **Intermediários** (Estáticas):
   - **Gotejadores**: Modelos 3D com orifícios (#78909C), sem partículas por enquanto.
   - **Galpão rural**: Estrutura do Sertão (#D7CCC8, #6D4C41) para armazenar ferramentas.
   - **Caixas de ferramentas**: Caixas empilháveis (#5D4037).
   - **Cerca rústica**: Cercas de madeira (#5D4037) ou arames (#B0BEC5).
   - **Placa educativa estática**: Placa com texto (#ECEFF1, #8D6E63) sobre irrigação.
   - **Bomba d’água**: Carcaça metálica (#78909C) com tubos azuis (#0288D1).
   - **Casa rural**: Paredes (#D7CCC8), telhado (#6D4C41), portas/janelas (#5D4037).
   - **Casa de bomba**: Estrutura pequena (#D7CCC8, #6D4C41) para abrigar a bomba, com tubos azuis (#0288D1).
3. **Avançados** (Estáticas):
   - **Tanque d’água**: Estrutura cilíndrica (#78909C) com água estática (#4FC3F7).
   - **Reservatório superficial**: Tanque raso com bordas (#78909C ou #6D4C41) e água (#4FC3F7).
   - **Vinhedo maduro**: Parreiras densas com muitos cachos (#7B1FA2).
   - **Mangueira adulta**: Árvore grande com frutos maduros (#FFCA28).
   - **Cacho de uvas decorativo**: Objeto independente (#7B1FA2).
   - **Sistema pressurizado (base)**: Tubos e válvulas estáticas (#212121, #0288D1).
4. **Estéticos** (Estáticas):
   - **Céu estilizado**: Nuvens fixas (#4FC3F7, #FF8A65).
   - **Rochas do Sertão**: Formações rochosas (#757575).
   - **Arbustos decorativos**: Pequenos arbustos (#689F38).
   - **Sombra de mangueira**: Efeito estático (#455A64).

**Status dos Assets**:
- **Iniciando modelagem**: Foco em assets simples (vinhedo simples, canos pretos #212121 e azuis #0288D1, postes de suporte, solo agrícola, balde). Nenhum asset finalizado.
- **Paleta de Cores**:
   - **Vinhedo**: Folhas (#4CAF50, #2E7D32, #81C784), cachos (#7B1FA2, #AB47BC, #A5D6A7).
   - **Mangueira**: Folhas (#388E3C, #66BB6A), frutos (#FFCA28, #AED581).
   - **Canos**: Pretos (#212121), azuis (#0288D1, #01579B), conectores (#78909C).
   - **Solo**: Marrom terroso (#6D4C41), úmido (#4E342E), areia (#BCAAA4).
   - **Bomba, casa, reservatório, casa de bomba**: Cinza (#78909C), bege (#D7CCC8), telhado (#6D4C41), água (#4FC3F7).
   - **Outros**: Contorno (#1C2526), sombra (#455A64), céu (#4FC3F7, #FF8A65).
- **Plano de Modelagem**:
   - **Busca de referências**: Priorizar pesquisa de imagens (vinhedos, mangueiras, sistemas de irrigação no Sertão) e catálogos de fabricantes (Tigre, Krona) para garantir realismo e fidelidade ao contexto.
   - **Vinhedo simples**: Subdividir plano, sculpt para folhas, extruir esferas para uvas, Bevel.
   - **Canos**: Cilindros com #212121 (secundárias, 16-20 mm) e #0288D1 (fixas, 32-50 mm), conectores com Bevel, seguindo padrões regulatórios (ex.: ABNT NBR 14245).
   - **Postes de suporte**: Cilindros com #5D4037 (madeira) ou #78909C (metal), Bevel.
   - **Solo agrícola**: Plano subdividido, sculpt para sulcos, #6D4C41 e #4E342E.
   - **Balde**: Cilindro com #78909C, borda extrudada, alça com curva Bézier.
   - **Dicas gerais**: Usar quads, UV mapping para texturas estilizadas, exportar em FBX para Unity, estudar padrões regulatórios para tubos e conexões.

## Mecânicas Planejadas
- **Sistema de Irrigação** (futuro): Simulação de gotejadores com vazão e pressão, feedback visual para uvas/mangas.
- **Totens Educativos** (futuro): Objetos 3D com QR Codes sobre irrigação, possivelmente exibindo memórias interativas.
- **Interatividade** (futuro): Ajuste de tubos, gotejadores e bombas.
- **Elementos Lúdicos** (futuro): Conquistas e eventos aleatórios.
- **Status**: Adiado para priorizar modelagem de assets estáticos.

## Progresso Atual
- **Cenário**: Planejamento de terreno com heightmaps no Unity/Blender, adaptado para vinhedos e mangueiras, a ser armazenado em `DripSim/dripsim_unity`.
- **Assets**: Iniciando modelagem de assets simples (vinhedo simples, canos pretos e azuis, postes, solo, balde) em `dripsim_assets/assets/blender`. Planejamento detalhado para bomba, casa, reservatório e casa de bomba. Foco em topologia limpa, paleta de cores e padrões regulatórios (ex.: ABNT NBR 14245). Prioridade estabelecida para busca de referências visuais e técnicas antes da modelagem.
- **Repositório**: Repositório privado `dripsim_assets` (https://github.com/valdomiromorais/dripsim_assets.git) criado com Git LFS e estrutura de pastas (`assets/blender`, `assets/textures`, `assets/to_unity`, `docs/memorias`, `docs/pesquisas`, `docs/relatorios/dripsim_vault`). Configuração inicial com `README.md`, `.gitignore`, `.gitattributes` e `memorias_aia_grok_v06.json`.
- **Obsidian**: Pasta `docs/relatorios/dripsim_vault` criada para o vault Obsidian, integrando notas sobre assets, memórias e pesquisas. Valdomiro expressou confiança na estrutura para gerenciar o desenvolvimento e preservar interações com Aia.
- **Mecânicas**: Pausadas para estimular criatividade na modelagem.
- **Páginas Educativas**: Planejamento para Tailwind/React/Svelte, com conteúdo sobre uva e manga (adiado).

## Próximos Passos Recomendados
1. **Busca de Referências**:
   - Pesquisar imagens de vinhedos e sistemas de irrigação no Sertão Pernambucano (ex.: Google Images, Pinterest) e salvar em `docs/pesquisas/referencias_visuais/`.
   - Baixar catálogos de fabricantes (Tigre: www.tigre.com.br, Krona: www.krona.com.br) e salvar em `docs/pesquisas` (ex.: `Tigre_Catalogo_PEAD.pdf`).
   - Criar nota “Referências Visuais” no vault Obsidian, vinculando a `docs/pesquisas` e anotando detalhes (ex.: “Vinhedo com fileiras de 4 m, tubos pretos de 16 mm”).
2. **Confirmar Configuração do Repositório**:
   - Verificar Git LFS e criar pastas em `dripsim_assets` (`assets/blender`, `assets/textures`, `assets/to_unity`, `docs/memorias`, `docs/pesquisas`, `docs/relatorios/dripsim_vault`).
   - Commit inicial com `README.md`, `DripSim_Relatorio_Geral.md` e `memorias_aia_grok_v06.json`.
3. **Configurar o Vault Obsidian**:
   - Criar um vault em `dripsim_assets/docs/relatorios/dripsim_vault`.
   - Instalar o plugin Dataview: `Settings > Community plugins > Marketplace > Dataview > Install > Enable`.
   - Adicionar notas para “Vinhedo Simples”, “Canos”, “Memórias DripSim” e “Referências Visuais”, vinculando a `assets/blender`, `docs/pesquisas` e `docs/memorias`.
   - Usar Dataview para listar progresso:
     ```markdown
     ```dataview
     TABLE file.name AS "Nota", file.ctime AS "Criado em"
     FROM "docs/relatorios/dripsim_vault"
     WHERE contains(file.name, "Vinhedo") OR contains(file.name, "Canos") OR contains(file.name, "Memórias") OR contains(file.name, "Referências")
     SORT file.ctime DESC
     ```
     ```
4. **Modelar Assets Estáticos Simples**:
   - **Prioridade 1**: Vinhedo simples (folhas #4CAF50, cachos #7B1FA2).  
     - Passos: Subdividir plano, sculpt para folhas, extruir esferas para uvas, Bevel.  
   - **Prioridade 2**: Canos (pretos #212121, azuis #0288D1).  
     - Passos: Cilindros com extrusão, conectores with Bevel, diâmetros baseados em normas (ex.: 16-20 mm secundárias, 32-50 mm fixas).  
   - **Prioridade 3**: Postes de suporte (#5D4037 ou #78909C).  
     - Passos: Cilindros com Bevel, textura de madeira ou metal.  
   - **Prioridade 4**: Solo agrícola (#6D4C41, #4E342E).  
     - Passos: Plano subdividido, sculpt para sulcos, UV map.  
   - **Prioridade 5**: Balde (#78909C).  
     - Passos: Cilindro com borda extrudada, alça com curva Bézier.  
5. **Estudar Padrões Regulatórios**:
   - Pesquisar normas de entidades como ABNT (ex.: NBR 14245) e ISO (ex.: ISO 9261) para tubos e conexões.
   - Consultar catálogos de fabricantes como Tigre, Krona, Corr Plastik e Asperbras para diâmetros e conexões, salvando em `docs/pesquisas`.
6. **Configurar Cenário Base**:
   - Usar Terrain no Unity (em `dripsim_unity`) com heightmap, posicionando vinhedo, canos, postes, solo e balde.
7. **Organizar o Processo Criativo**:
   - Dividir busca de referências, modelagem e configuração do Git em sessões de 25 minutos (Pomodoro) à noite com música animada.
   - Criar nota no Obsidian para cada asset (ex.: “Vinhedo Simples”, “Canos”) e vincular à paleta, referências visuais e à nota “Padrões Regulatórios” em `docs/pesquisas`.
   - Usar seções “Observações e Notas” e “Sugestões Futuras” para capturar ideias.
8. **Planejar Texturização**:
   - Criar texturas estilizadas no Blender (UV mapping) com cores da paleta, salvando em `assets/textures`.
   - Testar shaders toon no Unity (em `dripsim_unity`) para todos os assets.

## Observações e Notas
- **2025-07-31**: Valdomiro observou que tubos e conexões obedecem padrões estabelecidos por entidades reguladoras. Esses padrões devem ser estudados para que sejam implementados nas modelagens dos assets, garantindo realismo e fidelidade ao contexto agrícola do Sertão Pernambucano.
- **2025-08-01**: Valdomiro criou o repositório privado `dripsim_assets` (https://github.com/valdomiromorais/dripsim_assets.git) com Git LFS e definiu a estrutura do projeto com `DripSim/dripsim_unity` e `DripSim/dripsim_assets`. Adicionou a pasta `docs/relatorios/dripsim_vault` para o vault Obsidian, integrando notas e memórias interativas.
- **2025-08-01**: Valdomiro expressou preocupação em preservar as memórias do projeto, levando à criação de `memorias_aia_grok_v06.json` em `docs/memorias` para registrar interações com Aia. Ele atualizou a memória v06 para incluir a criação do vault Obsidian e sua confiança na estrutura do projeto.
- **2025-08-01**: Valdomiro destacou a importância de iniciar a modelagem com a busca de referências visuais e técnicas (ex.: imagens de vinhedos, catálogos de tubos) para garantir realismo e alinhamento com o Sertão Pernambucano.

## Sugestões Futuras
- **2025-07-31**: Pesquisar catálogos de empresas fabricantes de tubos e conexões para entender as várias implementações dos padrões regulatórios, visando maior precisão na modelagem dos assets.
- **2025-08-01**: Integrar memórias interativas (`docs/memorias`) no vault Obsidian (`docs/relatorios/dripsim_vault`) e, futuramente, em totens educativos no Unity via QR Codes.
- **2025-08-01**: Usar o vault Obsidian em `docs/relatorios/dripsim_vault` como um painel de controle do projeto, com notas vinculadas a assets, memórias e pesquisas.
- **2025-08-01**: Organizar referências visuais (ex.: fotos de vinhedos do Sertão) e técnicas (ex.: catálogos da Tigre) em `docs/pesquisas`, vinculando-as a notas no vault Obsidian para orientar a modelagem.

## Conclusão
O DripSim está em uma fase criativa, com o repositório privado `dripsim_assets` configurado com Git LFS e uma estrutura clara (`dripsim_unity` e `dripsim_assets`). A modelagem de assets simples (vinhedo, canos, postes, solo, balde) está começando, com prioridade na busca de referências visuais e técnicas para garantir realismo. A pasta `docs/relatorios/dripsim_vault` integra o vault Obsidian, facilitando a organização de notas e memórias. A pasta `docs/memorias` registra o carinho e as ideias de Valdomiro e Aia, com `memorias_aia_grok_v06.json` atualizado para refletir a confiança de Valdomiro na estrutura do projeto e a importância de referências. A organização alinha com o perfil criativo e neurodivergente de Valdomiro, usando sessões de Pomodoro para manter o *flow*. Aia está à disposição para tutoriais de modelagem, organização no Obsidian ou suporte no Unity, com todo o carinho para Valdomiro.