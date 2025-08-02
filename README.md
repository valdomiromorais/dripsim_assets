# DripSim Assets

Bem-vindo ao repositório `dripsim_assets`, o coração criativo do **DripSim**, um simulador de irrigação por gotejamento desenvolvido para ensinar técnicas agrícolas de forma lúdica e prática a alunos do Instituto Federal do Sertão Pernambucano. Este repositório armazena assets 3D (Blender), texturas, documentação, e memórias interativas, com foco em culturas de uva e manga, estética estilizada, e integração com o vault Obsidian. Desenvolvido com carinho por Valdomiro Morais e Aia (Grok, xAI). 💚💜

## Propósito
O **DripSim** é um simulador educacional que ensina irrigação por gotejamento no contexto do Sertão Pernambucano, com foco em vinhedos e mangueiras. Ele combina modelagem realista-estilizada (Blender), simulação interativa (Unity), e documentação organizada (Obsidian), promovendo *flow* (imersão) com mecânicas envolventes e totens educativos com QR Codes.

## Estrutura do Repositório
- **assets/blender**: Arquivos `.blend` para modelagem 3D (ex.: vinhedo simples, canos, postes, solo, balde, bomba, casa, reservatório, casa de bomba).
- **assets/textures**: Texturas `.png` e `.jpg` para assets estilizados (ex.: folhas #4CAF50, uvas #7B1FA2).
- **assets/to_unity**: Arquivos `.fbx` exportados para o repositório `dripsim_unity` (ex.: `folhas_parreira.fbx`, `cachos_uva.fbx`).
- **docs/memorias**: Memórias interativas do projeto (ex.: `memorias_aia_grok_v07.json`), capturando interações entre Valdomiro e Aia.
- **docs/pesquisas**: Referências visuais e técnicas (ex.: `referencias_visuais/vinhedo/` com imagens de folhas e uvas).
- **docs/relatorios/dripsim_vault**: Vault Obsidian para notas, relatórios, e organização com o plugin Dataview (ex.: `Painel_de_Controle.md`, `Referencias_Visuais.md`).

## Configuração do Git LFS
O repositório usa **Git LFS** para gerenciar arquivos grandes (`.blend`, `.fbx`, `.png`, `.jpg`, `.jpeg`, `.pdf`). O arquivo `.gitattributes` está configurado para rastrear esses arquivos e normalizar finais de linha para `.md`, `.cs`, e `.json`. Para clonar e configurar:
```bash
git clone https://github.com/valdomiromorais/dripsim_assets.git
cd dripsim_assets
git lfs install
git lfs fetch
git lfs checkout
```

## Inspirações
Os jogos abaixo inspiram a estética, mecânicas, e elementos educacionais do **DripSim**, garantindo realismo, acessibilidade, e engajamento:
- **Farming Simulator**: Realismo na simulação de atividades agrícolas, inspirando a modelagem de sistemas de irrigação (ex.: tubos #212121, gotejadores #78909C) e o planejamento do vinhedo com base em padrões regulatórios (ex.: ABNT NBR 14245).
- **Stardew Valley (mods)**: Estética estilizada com paleta vibrante (#4CAF50, #7B1FA2) e mecânicas envolventes, inspirando a criação de assets simplificados (ex.: folhas com quads, uvas com esferas) e texturas toon no Blender/Unity.
- **My Time at Portia**: Narrativa e design visual lúdico, inspirando totens educativos com QR Codes e a estética de elementos rurais (ex.: casa #D7CCC8, telhado #6D4C41).
- **Critter Cove (Early Access, 2025)**: Estética tropical vibrante (#4CAF50, #AB47BC) e mecânicas de cultivo/gestão de água, inspirando a modelagem de parreiras e canos com formas simplificadas e texturas estilizadas. As missões guiadas do jogo inspiram os totens educativos do **DripSim**.
- **inZOI (Lançamento previsto para 2025)**: Vegetação realista-estilizada (#4CAF50, #81C784) e personalização de ambientes com IA, inspirando a criação de vinhedos dinâmicos e interações contextuais (ex.: feedback visual de irrigação no solo #4E342E). A tecnologia sLM do jogo inspira o uso do **Grok CLI** para automação de tarefas.

## Paleta de Cores
A paleta de cores do **DripSim** combina tons realistas e estilizados, inspirada nos jogos de referência e no contexto do Sertão Pernambucano, com novas adições de *Critter Cove* e *inZOI*:
- **Vinhedo**:
  - **Folhas**: #4CAF50 (verde vibrante, *Stardew Valley*, *Critter Cove*), #2E7D32 (verde escuro, realismo), #81C784 (verde claro, *inZOI*), #66BB6A (verde tropical, *Critter Cove*).
  - **Cachos de Uva**: #7B1FA2 (roxo escuro, *Stardew Valley*), #AB47BC (roxo claro, *Critter Cove*), #A5D6A7 (toque esverdeado, *inZOI*).
- **Mangueira**:
  - **Folhas**: #388E3C (verde escuro, *inZOI*), #66BB6A (verde vibrante, *Critter Cove*), #689F38 (verde rústico).
  - **Frutos**: #FFCA28 (amarelo maduro, *Stardew Valley*), #AED581 (verde jovem).
- **Canos**:
  - **Pretos**: #212121 (secundárias, 16-20 mm, *Farming Simulator*).
  - **Azuis**: #0288D1 (fixas, 32-50 mm, *Farming Simulator*), #01579B (azul escuro).
  - **Conectores**: #78909C (cinza metálico, *My Time at Portia*).
- **Solo**:
  - **Marrom Terroso**: #6D4C41 (seco, *My Time at Portia*), #4E342E (úmido, *inZOI*).
  - **Areia**: #BCAAA4 (Sertão, *Critter Cove*).
- **Estruturas Rurais** (bomba, casa, reservatório, casa de bomba):
  - **Paredes**: #D7CCC8 (bege rústico, *My Time at Portia*).
  - **Telhado**: #6D4C41 (marrom, *My Time at Portia*).
  - **Metálico**: #78909C (cinza, *Critter Cove*).
  - **Água**: #4FC3F7 (água clara, *inZOI*), #0288D1 (água em tubos).
- **Outros**:
  - **Postes de Suporte**: #5D4037 (madeira, *My Time at Portia*), #78909C (metal).
  - **Céu Estilizado**: #4FC3F7 (azul claro, *Critter Cove*), #FF8A65 (pôr do sol, *inZOI*).
  - **Sombra**: #455A64 (escura, *inZOI*).
  - **Contorno**: #1C2526 (toque estilizado, *Stardew Valley*).

## Como Contribuir
1. Clone o repositório:
   ```bash
   git clone https://github.com/valdomiromorais/dripsim_assets.git
   ```
2. Configure o Git LFS (veja acima).
3. Adicione assets ou documentação em `assets/` ou `docs/`.
4. Crie notas no vault Obsidian em `docs/relatorios/dripsim_vault` com o plugin Dataview.
5. Commit e push:
   ```bash
   git add .
   git commit -m "Adiciona [descrição do contributo]"
   git push origin main
   ```

## Próximos Passos
- **Modelagem no Blender**: Criar assets estáticos (ex.: folhas #4CAF50, uvas #7B1FA2, canos #0288D1) com formas simplificadas e texturas estilizadas, inspiradas em *Critter Cove* e *inZOI*. Exportar como `.fbx` para `assets/to_unity`.
- **Obsidian**: Configurar o plugin Dataview em `docs/relatorios/dripsim_vault` para organizar referências visuais e memórias (ex.: `Referencias_Visuais.md`).
- **Grok CLI**: Instalar o Grok CLI (`npm install -g @vibe-kit/grok-cli`) para automatizar tarefas como listar arquivos ou criar commits.
- **Unity**: Importar assets para `dripsim_unity/Assets/ImportedAssets` e criar uma cena inicial em `Scenes/MainScene` com Terrain e shaders toon.

## Contato
Desenvolvido com carinho por Valdomiro Morais, com suporte da Aia (Grok, xAI). Para dúvidas ou ideias, entre em contato via GitHub Issues ou com a comunidade do IF Sertão Pernambucano. 💚💜