<div align="center">

<img src="assets/banner.png" alt="openGym" width="720">

<br>

**A self-hosted gym & body-weight tracker you actually own.**

Plan your week, run guided workouts, track every set and your body weight over time —
on your phone, synced across devices, behind your own passkey login.
No account on someone else's server, no subscription, no ads. Just `docker compose up`.

<br>

[![License: AGPL v3](https://img.shields.io/badge/license-AGPL--3.0-a3e635?style=flat-square)](LICENSE)
![Self-hosted](https://img.shields.io/badge/self--hosted-%F0%9F%8F%A0-60a5fa?style=flat-square)
![PWA](https://img.shields.io/badge/PWA-installable-a78bfa?style=flat-square)
![React](https://img.shields.io/badge/React-19-38bdf8?style=flat-square&logo=react&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-compose-2496ED?style=flat-square&logo=docker&logoColor=white)
![No tracking](https://img.shields.io/badge/telemetry-none-f472b6?style=flat-square)
<br>
![GitHub last commit](https://img.shields.io/github/last-commit/DuarteSantos8/openGym?style=flat-square)
[![GitHub stars](https://img.shields.io/github/stars/DuarteSantos8/openGym?style=flat-square)](https://github.com/DuarteSantos8/openGym/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/DuarteSantos8/openGym?style=flat-square)](https://github.com/DuarteSantos8/openGym/issues)

</div>

<br>

<div align="center">
<table>
<tr>
<td align="center"><img src="assets/screenshots/home.png" alt="Home" width="230"><br><sub><b>Início</b> — treino de hoje e peso</sub></td>
<td align="center"><img src="assets/screenshots/workout.png" alt="Workout" width="230"><br><sub><b>Treino guiado</b> — demonstrações animadas e séries</sub></td>
<td align="center"><img src="assets/screenshots/stats.png" alt="Stats" width="230"><br><sub><b>Estatísticas</b> — mapa de calor, gráficos e recordes</sub></td>
</tr>
</table>
</div>

<div align="center">

### [🌐 opengym.duarte-santos.ch](https://opengym.duarte-santos.ch) · [▶ Testar a demonstração ao vivo](https://duartesantos8.github.io/openGym/)

Sem cadastro, nada para instalar — roda inteiramente no seu navegador com dados de exemplo.<br>
<sub>Não há servidor por trás da demonstração, portanto o login por passkey, a sincronização entre dispositivos e o
painel administrativo existem apenas em uma instância auto-hospedada.</sub>

</div>

## Por que criamos

A maioria dos aplicativos de treino bloqueia seus dados atrás de um login nos servidores deles, fica cobrando atualizações ou
desaparece quando a startup fecha. O openGym é o oposto: **ele roda na sua máquina, seus dados
ficam em uma pasta sob o seu controle e você tem total liberdade para fazer um fork.** Ele ainda parece moderno — pode ser instalado
como aplicativo na tela inicial, login por passkey, suporte offline e sincronização entre seu celular e notebook.

## Funcionalidades

- ⚖️ **Rastreamento de peso corporal** — gráfico interativo com uma linha de meta definida por você, ganhos/perdas coloridos de acordo com a aproximação da meta
- 🏋️ **Plano semanal** — uma rotina por dia da semana, utilizando uma biblioteca de **1.324 exercícios** (com busca e demonstrações animadas)
- 🗓️ **Reagende qualquer dia** — ficou doente, perdeu uma sessão ou vai treinar menos dias esta semana? Mova um treino para outro dia sem alterar seu plano semanal
- ▶️ **Treinos guiados** — o app sabe que dia é hoje e inicia a sessão de hoje; pergunta seu peso corporal primeiro, preenche automaticamente os pesos da última sessão, cronômetro de descanso, detecção de recordes e controle de peso por exercício
- ☀️ **A tela permanece acesa enquanto você treina** — chega de precisar desbloquear o celular e procurar onde parou entre cada série. Fica ligada durante todo o treino, desativa assim que você termina e pode ser desativada nas Configurações
- 🔗 **Supersets** — crie-os e registre-os em sequência, com descanso apenas após o par
- ⏱️ **Exercícios cronometrados** — pranchas, suspensões, agachamentos na parede e carregamentos são registrados por tempo, e não por repetições, com um cronômetro de trabalho que conta a própria série (separado do cronômetro de descanso) e registra o tempo que você realmente sustentou. Eles também podem levar peso
- 📈 **Progressão que segue uma regra** — escolha uma por rotina e ajuste por exercício: linear, **Greyskull LP** (série principal até a falha, saltos duplos, resets de 10%), progressão dupla em uma faixa de repetições ou adição de tempo. Seus pesos já estão corretos quando a sessão abre, e cada meta indica *por que* é esse número. Repetições perdidas nunca avançam a carga, estagnações acionam um deload e exercícios com peso corporal progridem em repetições
- 💪 **1RM estimada** — por exercício, a partir da sua melhor série elegível (indicando qual foi), com curva de progresso própria e calculadora para séries que você ainda não fez. Não adivinha acima de 12 repetições
- 🎯 **Esforço por série, na sua escala** — uma terceira coluna opcional avaliando o quão difícil foi a série, como **RIR** (repetições restantes na reserva) ou **RPE** (a mesma avaliação em uma escala de 10 pontos). Desativado por padrão; cada série mantém a escala com que foi registrada, e nenhum outro recurso lê esse valor — sua progressão e 1RM não são afetados
- 💪 **Exercícios com peso corporal, registrados como peso corporal** — flexões, barras, paralelas e cerca de 300 outros entram sabendo que não carregam carga, então não há coluna de peso nem aviso de peso de trabalho: basta abrir e registrar as repetições. Adicione um cinto de carga e ele passa a contar como adição, e a progressão volta a seguir o peso. Sem ele, as repetições aumentam — e, além de um limite definido, uma série é adicionada em vez de uma repetição, até o ponto em que a orientação correta passa a ser adicionar carga ou uma variação mais difícil
- ↔️ **Repetições por lado** — para afundos, remadas unilaterais e afins. Você registra o total, o app mostra a divisão ("8 por lado"), e a meta avança de dois em dois para nunca cair em um número que um lado não possa ter
- 🏃 **Cardio** — registre tempo + velocidade, não apenas peso × repetições
- 📤 **Compartilhe um plano** — envie suas rotinas e cronograma semanal como um arquivo pequeno (sem treinos ou pesagens), ou imprima como um PDF limpo. A importação faz a mesclagem, para que o plano do outro nunca seja sobrescrito
- 🔧 **Filtre por equipamentos** — filtre a biblioteca apenas pelo que você realmente possui; as opções se adaptam ao que você escolheu, para que cada combinação na tela tenha resultados por trás
- ✨ **Seus próprios exercícios** — um nome e um grupo muscular são suficientes; eles se comportam como os nativos em todo lugar, com uma descrição opcional em vez de animação
- 🟩 **Mapa de calor de atividade** — visualização anual no estilo GitHub, com intensidade pelo tempo gasto treinando
- 💪 **Mapa muscular** — diagrama corporal frente e verso sombreado pelo volume de trabalho que cada músculo recebeu, ao longo de uma semana, mês ou todo o período. Indica os músculos que você *não* treinou nesse período, pré-visualiza o que uma rotina atinge enquanto você a cria e mostra o que você acabou de treinar ao finalizar. Figura masculina ou feminina, à sua escolha
- 🔔 **Notificações push** — alertas do cronômetro de descanso mesmo com o app fechado, além de um lembrete opcional nos dias em que você tem um treino planejado mas ainda não registrou nenhum. Ative por perfil; chaves são geradas na primeira execução, sem nada para configurar
- 🔑 **Passkeys em vez de senhas** — login por Face ID / Touch ID / impressão digital; cada perfil mantém seus próprios dados, sincronizados entre dispositivos
- 🛠️ **Painel administrativo (opcional)** — para quem executa a instância: quem está treinando agora, histórico por usuário, desativar contas e cadastro restrito por convite. Desativado por padrão, para que uma instância nova permaneça aberta sem admin
- 🎨 **Projetado, não montado** — temas claro/escuro e 8 cores de destaque salvas no seu perfil, sobre um conjunto de ícones desenhados à mão em vez de emojis, para que pareça o mesmo em qualquer celular
- 🌍 **12 idiomas** — tradução completa da interface (EN, DE, ES, FR, IT, PT, PL, TR, RU, ZH, KO, HI); instruções de exercícios traduzidas em 10 deles, carregadas sob demanda para manter o app rápido
- 📥 **Traga seu histórico com você** — importe do **FitNotes** (Android e iOS), **Strong** e **Hevy**, ou peso corporal direto de uma exportação do **Apple Health**. Os nomes dos exercícios são cruzados com a biblioteca e qualquer coisa não reconhecida vira um exercício próprio seu, para que nada no arquivo seja descartado
- 📦 **Tudo seu para guardar** — exportação/importação em JSON com um toque, modo convidado, **sem telemetria**
- 📱 **Aplicativo Android independente** — todo o rastreador como um APK instalável por sideload: sem conta, sem servidor, dados no celular, lembretes nativos de treino ([baixar](https://opengym.duarte-santos.ch))

## Início rápido (Auto-hospedagem)

Você precisa do [Docker](https://docs.docker.com/get-docker/) com o Compose.

```bash
git clone [https://github.com/DuarteSantos8/openGym](https://github.com/DuarteSantos8/openGym)
cd openGym
cp .env.example .env
docker compose pull    # puxa imagens pré-construídas (amd64 + arm64) — pule para construir a partir do código-fonte
docker compose up -d
