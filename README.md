# FisioBot — aplicativo web demonstrativo

Projeto escolar de apoio à organização de exercícios fisioterapêuticos domiciliares. **Não utiliza robô nem Arduino.** Possui dois perfis de demonstração: paciente e fisioterapeuta.

## Como abrir no VS Code

1. Extraia a pasta `fisiobot-vscode` do arquivo ZIP.
2. No VS Code, escolha **Arquivo > Abrir Pasta** e selecione `fisiobot-vscode`.
3. Abra `index.html` com a extensão **Live Server** (botão *Go Live*). Também é possível abrir `index.html` diretamente no navegador.
4. Na tela inicial, escolha **Paciente** ou **Fisioterapeuta**.

## Perfis e funcionalidades

### Fisioterapeuta
- Criar perfis demonstrativos de pacientes.
- Visualizar cada paciente e seu histórico de atividades registradas.
- Montar planos com exercícios da biblioteca, dias, horários, repetições e orientações.
- Remover uma atividade de um plano sem perder o histórico anterior.
- Alterar o nome do profissional no perfil.

### Paciente
- Visualizar as atividades previstas no dia.
- Consultar a biblioteca informativa e a rotina semanal.
- Iniciar uma atividade prescrita, controlar um cronômetro e registrar conclusão.
- Acompanhar gráficos simples e histórico de atividades concluídas.

## Como demonstrar na feira

1. Entre como **Fisioterapeuta** e abra o paciente fictício **Ana (demonstração)**.
2. Adicione uma atividade com dias e instruções.
3. Saia e entre como **Paciente**, selecionando a Ana.
4. Acesse **Rotina** e, se for um dos dias programados, inicie o exercício em **Meu dia**.
5. Conclua a atividade e veja o registro em **Evolução**.

## Estrutura da pasta

```text
fisiobot-vscode/
├── index.html
├── style.css
├── app.js
├── assets/
│   └── coala.svg
└── README.md
```

## Limitações importantes

- **Protótipo local**: tudo é guardado no `localStorage` do navegador, sem servidor. Os perfis não têm senhas reais nem autenticação. Em outro navegador ou dispositivo, os dados não são compartilhados.
- **Não armazene dados verdadeiros de saúde ou identificação de pacientes** nesta versão. Use nomes fictícios em demonstrações.
- O coala é apenas uma ilustração 2D, **não uma demonstração biomecânica correta** dos movimentos. As instruções e prescrições devem vir do fisioterapeuta.
- O botão de lembretes e o planejamento representam a rotina, mas **não enviam notificações automáticas**.
- Para uso real com pacientes, seria necessário desenvolver servidor seguro, autenticação, permissões, proteção de dados, validação clínica e outras salvaguardas.

Feito em HTML, CSS e JavaScript puro, sem dependências ou necessidade de instalação via npm.
