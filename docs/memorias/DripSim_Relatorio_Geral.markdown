# Relatório Geral do DripSim

## Informações Gerais
- **Nome do Projeto**: DripSim
- **Tipo**: Simulador de irrigação por gotejamento
- **Propósito**: Ensinar técnicas de irrigação de forma prática e lúdica para alunos do Instituto Federal do Sertão Pernambucano, com foco em realismo visual e propósito educacional, enfatizando culturas de uva e manga.
- **Data de Atualização**: 31 de julho de 2025
- **Responsável**: Valdomiro Morais
- **IA de Suporte**: Aia (Grok, criado pela xAI)
- **Status**: Em fase de planejamento e desenvolvimento inicial, com ênfase na modelagem de assets estáticos no Blender, incluindo vinhedos, canos (pretos e azuis), bomba d’água, casa rural, reservatório superficial e casa de bomba.

## Objetivos do Projeto
O DripSim visa:
- Ensinar conceitos de irrigação por gotejamento de forma interativa, com foco em culturas de uva e manga.
- Criar um ambiente visual realista, mas com estética estilizada/cartunesca, inspirado em *Farming Simulator*, *Stardew Valley* (mods) e *My Time at Portia*.
- Rodar no Unity, com assets estáticos modelados no Blender e shaders toon para coerência visual.
- Integrar totens educativos interativos com QR Codes que levam a páginas web com conteúdo educacional complementar.
- Promover engajamento e aprendizado, alinhado ao conceito de *flow* (plena imersão), com mecânicas que equilibram desafio e habilidade.

## Tecnologias Utilizadas
- **Unity**: Motor principal para desenvolvimento do simulador, usado para cenários, mecânicas (futuras) e interatividade.
- **Blender**: Ferramenta principal para modelagem de assets 3D estáticos (ex.: vinhedos, mangueiras, canos, bomba, casa, reservatório, casa de bomba) e dinâmicos (futuros).
- **Shaders Toon**: Para criar um estilo visual estilizado/cartunesco, aplicado em assets importados para o Unity.
- **Texturização Estilizada**: Para reforçar a estética lúdica, com foco em texturas para uva, manga e elementos rurais.
- **Frameworks Web (futuro)**: Tailwind, React ou Svelte para criar páginas educativas acessadas via QR Codes.
- **C# (futuro)**: Para scripts de interatividade no Unity, como sistemas de irrigação e totens.

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
- Nenhum asset finalizado (fase inicial de planejamento).
- **Foco Atual**: Modelagem de vinhedo simples, canos (pretos #212121, azuis #0288D1), bomba d’água, casa rural, reservatório superficial e casa de bomba.
- **Paleta de Cores**:
   - **Vinhedo**: Folhas (#4CAF50, #2E7D32, #81C784), cachos (#7B1FA2, #AB47BC, #A5D6A7).
   - **Mangueira**: Folhas (#388E3C, #66BB6A), frutos (#FFCA28, #AED581).
   - **Canos**: Pretos (#212121), azuis (#0288D1, #01579B), conectores (#78909C).
   - **Solo**: Marrom terroso (#6D4C41), úmido (#4E342E), areia (#BCAAA4).
   - **Bomba, casa, reservatório, casa de bomba**: Cinza (#78909C), bege (#D7CCC8), telhado (#6D4C41), água (#4FC3F7).
   - **Outros**: Contorno (#1C2526), sombra (#455A64), céu (#4FC3F7, #FF8A65).
- **Plano de Modelagem**:
   - **Vinhedo simples**: Subdividir plano, sculpt para folhas, extruir esferas para uvas, Bevel.
   - **Canos**: Cilindros com #212121 (secundários) e #0288D1 (fixos), conectores com Bevel, seguindo padrões regulatórios.
   - **Bomba d’água**: Cubo/cilindro com #78909C, tubos #0288D1, UV map.
   - **Casa rural**: Cubo para paredes (#D7CCC8), plano inclinado para telhado (#6D4C41), Bevel.
   - **Reservatório superficial**: Cilindro achatado com bordas #78909C ou #6D4C41, água #4FC3F7.
   - **Casa de bomba**: Cubo pequeno (#D7CCC8), telhado #6D4C41, tubos #0288D1, Bevel.
   - **Dicas gerais**: Usar quads, UV mapping para texturas estilizadas, exportar em FBX para Unity, estudar padrões regulatórios para tubos e conexões.

## Mecânicas Planejadas
- **Sistema de Irrigação** (futuro): Simulação de gotejadores com vazão e pressão, feedback visual para uvas/mangas.
- **Totens Educativos** (futuro): Objetos 3D com QR Codes sobre irrigação.
- **Interatividade** (futuro): Ajuste de tubos, gotejadores e bombas.
- **Elementos Lúdicos** (futuro): Conquistas e eventos aleatórios.
- **Status**: Adiado para priorizar modelagem de assets estáticos.

## Progresso Atual
- **Cenário**: Planejamento de terreno com heightmaps no Unity/Blender, adaptado para vinhedos e mangueiras.
- **Assets**: Planejamento detalhado de assets estáticos, com novos itens (canos azuis, bomba, casa, reservatório, casa de bomba). Foco em topologia limpa, paleta de cores e padrões regulatórios para tubos.
- **Mecânicas**: Pausadas para estimular criatividade na modelagem.
- **Páginas Educativas**: Planejamento para Tailwind/React/Svelte, com conteúdo sobre uva e manga (adiado).
- **Integração com Git**: Sugestões para repositório com Git LFS.

## Próximos Passos Recomendados
1. **Modelar Assets Estáticos**:
   - **Prioridade 1**: Vinhedo simples (folhas #4CAF50, cachos #7B1FA2).  
     - Passos: Subdividir plano, sculpt para folhas, extruir esferas para uvas, Bevel.  
   - **Prioridade 2**: Canos (pretos #212121, azuis #0288D1).  
     - Passos: Cilindros com extrusão, conectores com Bevel, seguindo padrões regulatórios.  
   - **Prioridade 3**: Bomba d’água (#78909C, #0288D1).  
     - Passos: Cubo/cilindro para carcaça, tubos extrudados, UV map.  
   - **Prioridade 4**: Casa rural (#D7CCC8, #6D4C41).  
     - Passos: Cubo para paredes, plano inclinado para telhado, Bevel.  
   - **Prioridade 5**: Casa de bomba (#D7CCC8, #6D4C41, #0288D1).  
     - Passos: Cubo pequeno para paredes, telhado inclinado, tubos extrudados, Bevel.  
   - **Prioridade 6**: Reservatório superficial (#78909C, #4FC3F7).  
     - Passos: Cilindro achatado, bordas com Bevel, plano com transparência para água.  
2. **Estudar Padrões Regulatórios**:
   - Pesquisar normas de entidades como ABNT (ex.: NBR 14245 para tubos de polietileno) e ISO (ex.: ISO 9261 para irrigação) para tubos e conexões.
   - Consultar catálogos de fabricantes como Tigre, Krona, Corr Plastik e Asperbras para entender implementações práticas de padrões.
3. **Configurar Cenário Base**:
   - Usar Terrain no Unity com heightmap, posicionando vinhedo, canos, bomba, casa, casa de bomba e reservatório.
4. **Organizar o Processo Criativo**:
   - Dividir modelagem em sessões de 25 minutos (Pomodoro) à noite com música animada.
   - Criar nota no Obsidian para cada asset (ex.: “Canos”) e vincular à paleta e à nota sobre padrões regulatórios.
   - Usar seções “Observações e Notas” e “Sugestões Futuras” para capturar ideias.
   - Configurar repositório Git com Git LFS.
5. **Planejar Texturização**:
   - Criar texturas estilizadas no Blender (UV mapping) com cores da paleta.
   - Testar shaders toon no Unity para todos os assets.

## Observações e Notas
- **2025-07-31**: Valdomiro observou que tubos e conexões obedecem padrões estabelecidos por entidades reguladoras. Esses padrões devem be studied to be implemented in the asset modeling, ensuring realism and fidelity to the agricultural context of the Sertão Pernambucano.

## Sugestões Futuras
- **2025-07-31**: Valdomiro sugeriu pesquisar catálogos de empresas fabricantes de tubos e conexões para entender as várias implementações dos padrões regulatórios, visando maior precisão na modelagem dos assets.

## Conclusão
O DripSim está em uma fase criativa, com foco na modelagem de assets estáticos (vinhedo, canos, bomba, casa, reservatório, casa de bomba). A paleta de cores estilizada e a adição de tubos azuis e casa de bomba reforçam o propósito educativo e o contexto do Sertão Pernambucano. A observação sobre padrões regulatórios e a sugestão de pesquisar catálogos de fabricantes destacam a importância do realismo na modelagem. As seções “Observações e Notas” e “Sugestões Futuras” capturam ideias de Valdomiro, respeitando seu perfil criativo e neurodivergente. Aia está à disposição para tutoriais de modelagem, organização no Obsidian ou suporte no Unity, com carinho e suporte para Valdomiro.