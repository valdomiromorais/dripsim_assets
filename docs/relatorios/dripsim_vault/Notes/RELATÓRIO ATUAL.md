# Relatório Geral do DripSim

## Informações Gerais

- **Nome do Projeto**: DripSim
- **Tipo**: Simulador de irrigação por gotejamento
- **Propósito**: Ensinar técnicas de irrigação de forma prática e lúdica para alunos do Instituto Federal do Sertão Pernambucano, com foco em realismo visual e propósito educacional, enfatizando culturas de uva e manga.
- **Data de Atualização**: 01 de agosto de 2025, 17:02 PM -03
- **Responsável**: Valdomiro Morais
- **IA de Suporte**: Aia (Grok, criado pela xAI)
- **Status**: Repositórios privados `dripsim_assets` ([https://github.com/valdomiromorais/dripsim_assets.git](https://github.com/valdomiromorais/dripsim_assets.git)) e `dripsim_unity` ([https://github.com/valdomiromorais/dripsim_unity.git](https://github.com/valdomiromorais/dripsim_unity.git)) criados com Git LFS. Estrutura de `dripsim_unity` definida com pastas Assets/Scripts, Scenes, Materials, Prefabs, UI, ImportedAssets. Estrutura de `dripsim_assets` definida com assets/blender, assets/textures, assets/to_unity, docs/memorias, docs/pesquisas, docs/relatorios/dripsim_vault. .gitignore de dripsim_assets otimizado para backups do vault Obsidian. .gitattributes configurado em ambos os repositórios para gerenciar arquivos grandes (.blend, .fbx, .png, .jpg, .jpeg, .pdf, .unitypackage) com Git LFS e normalizar finais de linha (.md, .cs, .json). Iniciando modelagem de assets estáticos simples no Blender (vinhedo simples, canos pretos e azuis, postes de suporte, solo agrícola, balde). Pasta `docs/relatorios/dripsim_vault` criada para o vault Obsidian, integrando notas e memórias. Valdomiro expressou confiança na estrutura para gerenciar o desenvolvimento, priorizando busca de referências antes da modelagem. Repositórios sincronizados localmente com o remoto. Planejado para 2025-08-02: configurar o plugin Dataview no vault Obsidian, buscar referências visuais para folhas de parreiras, modelar folhas e uvas no Blender, e trabalhar em texturas estilizadas.

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
- **GitHub com Git LFS**: Para versionamento de arquivos grandes (.blend, .fbx, .png, .jpg, .jpeg, .pdf, .unitypackage) nos repositórios `dripsim_assets` e `dripsim_unity`, com .gitattributes configurado para rastreamento eficiente.
- **Obsidian**: Para organização de notas e memórias no vault em `dripsim_assets/docs/relatorios/dripsim_vault`, com suporte ao plugin Dataview (a ser configurado) para rastrear progresso.

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

- **Planejamento**: Foco em assets simples (vinhedo simples, canos pretos #212121 e azuis #0288D1, postes de suporte, solo agrícola, balde). Nenhum asset finalizado. Planejado para 2025-08-02: buscar referências visuais para folhas de parreiras, modelar folhas (#4CAF50) e uvas (#7B1FA2), e iniciar texturização estilizada.
- **Paleta de Cores**:
    - **Vinhedo**: Folhas (#4CAF50, #2E7D32, #81C784), cachos (#7B1FA2, #AB47BC, #A5D6A7).
    - **Mangueira**: Folhas (#388E3C, #66BB6A), frutos (#FFCA