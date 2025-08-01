# Relatório Geral do DripSim

## Informações Gerais

- **Nome do Projeto**: DripSim
- **Tipo**: Simulador de irrigação por gotejamento
- **Propósito**: Ensinar técnicas de irrigação de forma prática e lúdica para alunos do Instituto Federal do Sertão Pernambucano, com foco em realismo visual e propósito educacional, enfatizando culturas de uva e manga.
- **Data de Atualização**: 01 de agosto de 2025, 16:33 PM -03
- **Responsável**: Valdomiro Morais
- **IA de Suporte**: Aia (Grok, criado pela xAI)
- **Status**: Repositórios privados `dripsim_assets` ([https://github.com/valdomiromorais/dripsim_assets.git](https://github.com/valdomiromorais/dripsim_assets.git)) e `dripsim_unity` ([https://github.com/valdomiromorais/dripsim_unity.git](https://github.com/valdomiromorais/dripsim_unity.git)) criados com Git LFS. Estrutura de `dripsim_unity` definida com pastas Assets/Scripts, Scenes, Materials, Prefabs, UI, ImportedAssets. Estrutura de `dripsim_assets` definida com assets/blender, assets/textures, assets/to_unity, docs/memorias, docs/pesquisas, docs/relatorios/dripsim_vault. .gitignore de dripsim_assets otimizado para backups do vault Obsidian. Iniciando modelagem de assets estáticos simples no Blender (vinhedo simples, canos pretos e azuis, postes de suporte, solo agrícola, balde). Pasta `docs/relatorios/dripsim_vault` criada para o vault Obsidian, integrando notas e memórias. Valdomiro expressou confiança na estrutura para gerenciar o desenvolvimento, priorizando busca de referências antes da modelagem. Repositórios sincronizados localmente com o remoto.

## Objetivos do Projeto

O DripSim visa:

- Ensinar conceitos de irrigação por gotejamento de forma interativa, com foco em culturas de uva e manga.
- Criar um ambiente visual realista, mas com estética estilizada/cartunesca, inspirado em _Farming Simulator_, _Stardew Valley_ (mods) e _My Time at Portia_.
- Rodar no Unity, com assets estáticos modelados no Blender e shaders toon para coerência visual.
- Integrar totens educativos interativos com QR Codes que levam a páginas web com conteúdo educacional complementar.
- Promover engajamento e aprendizado, alinhado ao conceito de _flow_ (plena imersão), com mecânicas que equilibram desafio e habilidade.

## Tecnologias Utilizadas

- **Unity 6**: Motor principal para desenvolvimento do simulador, usado para cenários, mecânicas (futuras) e interatividade, armazenado em `DripSim/dripsim_unity`.
- **Blender**: Ferramenta principal para modelagem de assets 3D estáticos (ex.: vinhedos, mangueiras, canos, bomba, casa, reservatório, casa de bomba) e dinâmicos (futuros), armazenados em `dripsim_assets/assets/blender`.
- **Shaders Toon**: Para criar um estilo visual estilizado/cartunesco, aplicado em assets importados para o Unity.
- **Texturização Estilizada**: Para reforçar a estética lúdica, com foco em texturas para uva, manga e elementos rurais, armazenadas em `dripsim_assets/assets/textures`.
- **Frameworks Web (futuro)**: Tailwind, React ou Svelte para criar páginas educativas acessadas via QR Codes.
- **C# e Visual Scripting**: Para scripts de interatividade no Unity, como sistemas de irrigação e totens.
- **GitHub com Git LFS**: Para versionamento de arquivos grandes (.blend, .fbx, .png, .unitypackage) nos repositórios `dripsim_assets` e `dripsim_unity`.
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

- **Cenário**: Planejamento de terreno com heightmaps no Unity/Blender, adaptado para vinhedos e mangueiras, a ser armazenado em `dripsim_unity/Scenes`.
- **Assets**: Iniciando modelagem de assets simples (vinhedo simples, canos pretos e azuis, postes, solo, balde) em `dripsim_assets/assets/blender`. Planejamento detalhado para bomba, casa, reservatório e casa de bomba. Foco em topologia limpa, paleta de cores e padrões regulatórios (ex.: ABNT NBR 14245). Prioridade estabelecida para busca de referências visuais e técnicas antes da modelagem.
- **Repositórios**: Repositório privado `dripsim_assets` ([https://github.com/valdomiromorais/dripsim_assets.git](https://github.com/valdomiromorais/dripsim_assets.git)) criado com Git LFS para assets e documentação (`assets/blender`, `assets/textures`, `assets/to_unity`, `docs/memorias`, `docs/pesquisas`, `docs/relatorios/dripsim_vault`). .gitignore otimizado para backups do vault Obsidian. Repositório privado `dripsim_unity` ([https://github.com/valdomiromorais/dripsim_unity.git](https://github.com/valdomiromorais/dripsim_unity.git)) criado para projeto Unity, com estrutura definida (Assets/Scripts, Scenes, Materials, Prefabs, UI, ImportedAssets) e README.md detalhado. Repositórios sincronizados localmente com o remoto.
- **Obsidian**: Pasta `docs/relatorios/dripsim_vault` criada em `dripsim_assets` para o vault Obsidian, integrando notas sobre assets, memórias e pesquisas. Valdomiro expressou confiança na estrutura para gerenciar o desenvolvimento e preservar interações com Aia.
- **Mecânicas**: Pausadas para estimular criatividade na modelagem.
- **Páginas Educativas**: Planejamento para Tailwind/React/Svelte, com conteúdo sobre uva e manga (adiado).

## Próximos Passos Recomendados

1. **Configurar o Vault Obsidian**:
    - Criar um vault em `dripsim_assets/docs/relatorios/dripsim_vault`.
    - Instalar o plugin Dataview: `Settings > Community plugins > Marketplace > Dataview > Install > Enable`.
    - Adicionar notas para “Vinhedo Simples”, “Canos”, “Memórias DripSim” e “Referências Visuais”, vinculando a `assets/blender`, `docs/pesquisas` e `docs/memorias`.
    - Criar uma nota `Painel de Controle.md`:
        
        ````markdown
        ---
        tags: [painel]
        status: em_andamento
        criado_em: 2025-08-01
        ---
        ## Painel de Controle do DripSim
        ### Notas sobre Assets, Memórias e Referências
        ```dataview
        TABLE file.name AS "Nota", file.ctime AS "Criado em"
        FROM "docs/relatorios/dripsim_vault"
        WHERE contains(file.name, "Vinhedo") OR contains(file.name, "Canos") OR contains(file.name, "Memórias") OR contains(file.name, "Referências")
        SORT file.ctime DESC
        ````
        
    - Commit:
        
        ```bash
        git add dripsim_assets/docs/relatorios/dripsim_vault/Painel\ de\ Controle.md
        git commit -m "Adiciona Painel de Controle com Dataview no vault Obsidian"
        git push origin main
        ```
        
2. **Busca de Referências**:
    - Pesquisar imagens de vinhedos e sistemas de irrigação no Sertão Pernambucano (ex.: Google Images, Pinterest, Embrapa Uva e Vinho: [www.embrapa.br/uva-e-vinho](http://www.embrapa.br/uva-e-vinho)) e salvar em `dripsim_assets/docs/pesquisas/referencias_visuais/`.
    - Baixar catálogos de fabricantes (Tigre: [www.tigre.com.br](http://www.tigre.com.br/), Krona: [www.krona.com.br](http://www.krona.com.br/)) e salvar em `dripsim_assets/docs/pesquisas` (ex.: `Tigre_Catalogo_PEAD_2025.pdf`).
    - Criar nota “Referências Visuais” no vault Obsidian:
        
        ```markdown
        ---
        tags: [referencias, vinhedo, canos]
        status: em_andamento
        criado_em: 2025-08-01
        ---
        # Referências Visuais
        - **Vinhedo**: Fileiras de 4 m, folhas #4CAF50, cachos #7B1FA2. Arquivos: [[../../docs/pesquisas/referencias_visuais/vinhedo/vinhedo_ref_01.jpg]]
        - **Canos**: Tubos pretos 16-20 mm #212121, azuis 32-50 mm #0288D1. Arquivo: [[../../docs/pesquisas/Tigre_Catalogo_PEAD_2025.pdf]]
        ```
        
    - Commit:
        
        ```bash
        mkdir -p dripsim_assets/docs/pesquisas/referencias_visuais/vinhedo
        git add dripsim_assets/docs/pesquisas dripsim_assets/docs/relatorios/dripsim_vault
        git commit -m "Adiciona referências visuais e técnicas para vinhedo e canos"
        git push origin main
        ```
        
3. **Modelar Assets Estáticos Simples**:
    - **Prioridade 1**: Vinhedo simples (folhas #4CAF50, cachos #7B1FA2).
        - Passos: Subdividir plano (Shift+A > Mesh > Plane, Ctrl+R, 10 cortes), sculpt com pincel **Grab** para folhas, extruir esferas (Shift+A > Mesh > UV Sphere) para uvas, Bevel (Ctrl+B). Salvar em `dripsim_assets/assets/blender/vinhedo.blend` e exportar como `vinhedo.fbx` para `dripsim_assets/assets/to_unity`.
    - **Prioridade 2**: Canos (pretos #212121, azuis #0288D1).
        - Passos: Cilindros (Shift+A > Mesh > Cylinder, 16 lados) com extrusão (E), diâmetros 16-20 mm (secundárias) e 32-50 mm (fixas), conectores (#78909C) com Boolean e Bevel, seguindo normas (ex.: ABNT NBR 14245). Salvar em `dripsim_assets/assets/blender/canos.blend` e exportar como `canos.fbx`.
    - **Prioridade 3**: Postes de suporte (#5D4037 ou #78909C).
        - Passos: Cilindros com Bevel, textura de madeira ou metal.
    - **Prioridade 4**: Solo agrícola (#6D4C41, #4E342E).
        - Passos: Plano subdividido, sculpt para sulcos, UV map.
    - **Prioridade 5**: Balde (#78909C).
        - Passos: Cilindro com borda extrudada, alça com curva Bézier.
    - Commit:
        
        ```bash
        git add dripsim_assets/assets/blender/vinhedo.blend dripsim_assets/assets/to_unity/vinhedo.fbx
        git commit -m "Inicia modelagem do vinhedo simples com folhas #4CAF50 e cachos #7B1FA2"
        git push origin main
        ```
        
4. **Estudar Padrões Regulatórios**:
    - Pesquisar normas de entidades como ABNT (ex.: NBR 14245) e ISO (ex.: ISO 9261) para tubos e conexões.
    - Consultar catálogos de fabricantes como Tigre, Krona, Corr Plastik e Asperbras, salvando em `dripsim_assets/docs/pesquisas`.
5. **Configurar Cenário Base no Unity**:
    - Criar uma cena `MainScene` em `dripsim_unity/Scenes` com Terrain (heightmap).
    - Importar assets de `dripsim_assets/assets/to_unity` (ex.: `vinhedo.fbx`, `canos.fbx`) para `dripsim_unity/Assets/ImportedAssets`.
    - Commit:
        
        ```bash
        cd DripSim/dripsim_unity
        git add Scenes Assets/ImportedAssets
        git commit -m "Configura cena inicial MainScene com assets importados"
        git push origin main
        ```
        
6. **Organizar o Processo Criativo**:
    - Dividir busca de referências, configuração do Dataview, modelagem e commits em sessões de 25 minutos (Pomodoro) à noite com música animada.
    - Criar nota no Obsidian para cada asset (ex.: “Vinhedo Simples”, “Canos”) e vincular à paleta, referências visuais e à nota “Padrões Regulatórios