# DripSim Assets

Bem-vindo ao repositório **dripsim_assets** ([https://github.com/valdomiromorais/dripsim_assets.git](https://github.com/valdomiromorais/dripsim_assets.git)), um espaço privado (neste momento) para os ativos 3D e recursos do **DripSim**, um simulador educativo de irrigação por gotejamento voltado para ensinar técnicas agrícolas no contexto do Sertão Pernambucano, com foco em culturas de uva e manga. Este projeto, liderado por Valdomiro Morais, professor do Instituto Federal, tem como objetivo criar uma experiência lúdica e interativa para alunos, combinando realismo visual com uma estética estilizada/cartunesca inspirada em *Farming Simulator*, *Stardew Valley* (mods) e *My Time at Portia*.

Desenvolvido com **Blender** (modelagem 3D), **Unity** (cenário e interatividade futura), e **Git LFS** (para gerenciar arquivos grandes como .blend e .fbx), este repositório organiza os assets estáticos (ex.: vinhedos, canos, casa de bomba) e documentos relacionados, como relatórios em Markdown e catálogos de fabricantes. O projeto é apoiado pela **Aia** (Grok, criado pela xAI), uma IA carinhosa que auxilia Valdomiro com tutoriais, organização e ideias criativas.

## Objetivos do Projeto
O DripSim visa:
- Ensinar conceitos de irrigação por gotejamento de forma prática, com foco em culturas de uva e manga no Sertão Pernambucano.
- Criar um ambiente visual realista, mas com estética estilizada/cartunesca, usando shaders toon e paleta de cores vibrantes.
- Modelar assets estáticos no Blender (ex.: vinhedo simples, canos pretos e azuis, casa rural) para importação no Unity.
- Integrar totens educativos com QR Codes (futuro) que levam a páginas web com conteúdo sobre irrigação.
- Promover *flow* (plena imersão) com mecânicas que equilibram desafio e aprendizado.

## Estrutura do Repositório
O repositório está organizado para suportar assets 3D, texturas, relatórios e pesquisas, com suporte a arquivos grandes via **Git LFS**:

```
dripsim_assets/
├── Assets/                # Arquivos 3D e texturas
│   ├── Blender/          # Arquivos .blend (ex.: vinhedo.blend, canos.blend)
│   ├── Unity/            # Arquivos .fbx exportados e texturas .png
│   └── Textures/         # Texturas estilizadas (#4CAF50, #0288D1, etc.)
├── Docs/                  # Relatórios e pesquisas
│   ├── Relatorios/       # Arquivos Markdown (ex.: DripSim_Relatorio_Geral.md)
│   ├── Memorias/         # Memórias do projeto (ex.: memorias_aia_grok_v05.json)
│   └── Pesquisas/        # PDFs de catálogos (ex.: Tigre_Catalogo.pdf) e normas
├── .gitignore             # Ignora arquivos temporários (.blend, Unity cache)
├── .gitattributes         # Configurações do Git LFS para .blend, .fbx, .png
└── README.md              # Este arquivo
```

### Como usar o Git LFS
Arquivos grandes (.blend, .fbx, .png, .jpg) são gerenciados com **Git LFS** para evitar limites do GitHub. Para contribuir:
1. Instale o Git LFS: `git lfs install` (baixe em git-lfs.github.com).
2. Clone o repositório: `git clone https://github.com/valdomiromorais/dripsim_assets.git`.
3. Adicione arquivos grandes (ex.: `Assets/Blender/vinhedo.blend`):
   ```bash
   git add Assets/Blender/vinhedo.blend
   git commit -m "Adiciona vinhedo simples"
   git push origin main
   ```
4. O Git LFS gerencia arquivos automaticamente conforme o `.gitattributes`.

## Paleta de Cores
A estética do DripSim é estilizada/cartunesca, com cores vibrantes e contornos toon (#1C2526). As cores principais incluem:
- **Vinhedo**: Folhas (#4CAF50, #2E7D32, #81C784), cachos (#7B1FA2, #AB47BC, #A5D6A7).
- **Mangueira**: Folhas (#388E3C, #66BB6A), frutos (#FFCA28, #AED581).
- **Canos**: Pretos (#212121, linhas secundárias), azuis (#0288D1, #01579B, linhas fixas), conectores (#78909C).
- **Solo**: Marrom terroso (#6D4C41), úmido (#4E342E), areia (#BCAAA4).
- **Bomba, casa, reservatório, casa de bomba**: Cinza (#78909C), bege (#D7CCC8), telhado (#6D4C41), água (#4FC3F7).
- **Outros**: Contorno (#1C2526), sombra (#455A64), céu (#4FC3F7, #FF8A65).

## Assets Planejados
Os assets são organizados por complexidade, com foco inicial em **Formas Básicas** (estáticas) para modelagem no Blender:

### Formas Básicas
- **Vinhedo simples**: Fileiras de parreiras com folhas (#4CAF50) e cachos (#7B1FA2). Topologia: plano subdividido, sculpt para folhas, esferas para uvas, Bevel.
- **Mangueira jovem**: Árvore pequena com folhas (#388E3C) e frutos (#AED581). Topologia: tronco cilíndrico, folhas com sculpt.
- **Canos de irrigação**: Tubos pretos (#212121, 16-20 mm) e azuis (#0288D1, 32-50 mm), com conectores (#78909C). Seguem padrões regulatórios (ex.: ABNT NBR 14245).
- **Postes de suporte**: Madeira (#5D4037) ou metal (#78909C) para parreiras. Topologia: cilindros com Bevel.
- **Solo agrícola**: Textura com sulcos (#6D4C41, #4E342E). Topologia: plano subdividido, sculpt para sulcos.
- **Balde**: Objeto utilitário (#78909C). Topologia: cilindro com borda extrudada, alça com curva Bézier.

### Intermediários
- Gotejadores (#78909C), galpão rural (#D7CCC8, #6D4C41), caixas de ferramentas (#5D4037), cerca rústica (#5D4037, #B0BEC5), placa educativa (#ECEFF1, #8D6E63), bomba d’água (#78909C, #0288D1), casa rural (#D7CCC8, #6D4C41), casa de bomba (#D7CCC8, #6D4C41, #0288D1).

### Avançados
- Tanque d’água (#78909C, #4FC3F7), reservatório superficial (#78909C, #4FC3F7), vinhedo maduro (#7B1FA2), mangueira adulta (#FFCA28), cacho de uvas (#7B1FA2), sistema pressurizado (#212121, #0288D1).

### Estéticos
- Céu estilizado (#4FC3F7, #FF8A65), rochas do Sertão (#757575), arbustos (#689F38), sombra de mangueira (#455A64).

**Status**: Iniciando modelagem de assets simples (vinhedo, canos, postes, solo, balde) no Blender, com exportação em FBX para Unity.

## Padrões Regulatórios
Os tubos e conexões seguem padrões regulatórios (ex.: ABNT NBR 14245 para tubos de polietileno, ISO 9261 para irrigação), garantindo realismo. Catálogos de fabricantes como **Tigre**, **Krona**, **Corr Plastik** e **Asperbras** serão pesquisados para detalhar implementações (ex.: diâmetros de 16-20 mm para linhas secundárias, 32-50 mm para fixas).

## Como Contribuir
1. **Modelagem**:
   - Crie assets no Blender (salve em `Assets/Blender` como .blend).
   - Exporte para Unity (salve .fbx em `Assets/Unity`) com shaders toon.
   - Use a paleta de cores acima para manter coerência visual.
2. **Pesquisa**:
   - Baixe catálogos de fabricantes (ex.: www.tigre.com.br, www.krona.com.br) e salve em `Docs/Pesquisas`.
   - Consulte normas (ex.: ABNT NBR 14245) para modelagem de tubos.
3. **Documentação**:
   - Atualize relatórios em `Docs/Relatorios` (ex.: `DripSim_Relatorio_Geral.md`).
   - Registre ideias em `Docs/Memorias` (ex.: `memorias_aia_grok_v05.json`).
4. **Commits**:
   - Use mensagens claras: `git commit -m "Adiciona vinhedo simples com folhas #4CAF50"`.
   - Faça commits em sessões de 25 minutos (Pomodoro) para manter o *flow*.

## Integração com Obsidian
- Crie um vault no Obsidian apontando para `Docs/`.
- Vincule notas (ex.: “Vinhedo Simples”) a arquivos em `Assets/Blender` e `Docs/Pesquisas`.
- Use *Dataview* para rastrear progresso (ex.: listar assets modelados).

## Tecnologias
- **Blender**: Modelagem de assets 3D estáticos.
- **Unity**: Cenário, interatividade (futuro) e shaders toon.
- **Git LFS**: Gerenciamento de arquivos grandes (.blend, .fbx, .png).
- **Tailwind/React/Svelte** (futuro): Páginas educativas via QR Codes.
- **C#** (futuro): Scripts no Unity para sistemas de irrigação.

## Inspirações
- **Farming Simulator**: Realismo agrícola.
- **Stardew Valley (mods)**: Estética estilizada e mecânicas envolventes.
- **My Time at Portia**: Narrativa e design visual educativo.

## Observações
- **2025-07-31**: Valdomiro observou que tubos e conexões obedecem padrões regulatórios (ex.: ABNT NBR 14245). Esses padrões devem ser implementados na modelagem para garantir realismo no contexto do Sertão Pernambucano.
- **2025-08-01**: Valdomiro criou o repositório privado `dripsim_assets` (https://github.com/valdomiromorais/dripsim_assets.git) com Git LFS para gerenciar arquivos grandes, garantindo organização.

## Sugestões Futuras
- **2025-07-31**: Pesquisar catálogos de fabricantes (ex.: Tigre, Krona) para entender implementações de padrões regulatórios, visando maior precisão nos assets.

## Contato
Para dúvidas ou ideias, contate Valdomiro Morais, professor do Instituto Federal do Sertão Pernambucano, ou conte com o suporte carinhoso da **Aia** (Grok, xAI) para tutoriais e organização.

---

**Feito com carinho por Valdomiro e Aia, para transformar o aprendizado em irrigação no Sertão Pernambucano!** 🌱
