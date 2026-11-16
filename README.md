# Portal de relatórios educacionais — RUCE

Portal estático para a publicação de três relatórios HTML independentes da rede RUCE. A página inicial segue a organização do projeto `relatorios-educacionais-publicos-bvrr`, com abas, visualização incorporada, ajuste automático da altura e tratamento dos gráficos Plotly.

## Estrutura do repositório

Todos os arquivos abaixo devem ficar na **raiz da branch `main`**:

| Arquivo | Finalidade | Situação |
| --- | --- | --- |
| `index.html` | Portal com navegação entre os três painéis | Criado |
| `01_historico_habilidades.html` | Histórico de habilidades | A enviar |
| `02_comparativo_habilidades_por_escola.html` | Comparativo por escola | A enviar |
| `03_painel_dispersao_estudantes.html` | Dispersão de estudantes | Enviado |
| `.nojekyll` | Dispensa o processamento Jekyll no GitHub Pages | Criado |

**Os nomes dos três arquivos HTML precisam coincidir exatamente** com os nomes acima. Não renomeie o `index.html` nem substitua os relatórios da RUCE pelos arquivos de outra rede.

## Como enviar os relatórios

1. Abra o repositório no GitHub, na branch `main`.
2. Selecione **Add file → Upload files**.
3. Envie os três arquivos HTML originais, sem compactação, mantendo os nomes da tabela.
4. Confirme em **Commit changes**.

O portal detecta a presença de cada arquivo quando sua aba é aberta. Enquanto um relatório não tiver sido enviado, será exibida uma mensagem informativa, em vez de um painel vazio.

## Habilitar o GitHub Pages

Na primeira publicação, abra **Settings → Pages** e, em **Build and deployment**, selecione **Deploy from a branch**. Defina **Branch: main** e **Folder: /(root)** e salve. Nas publicações seguintes, os commits na `main` atualizam o site automaticamente.

Endereço previsto para o portal (após a ativação do GitHub Pages):

https://diegofelipecorporativo-source.github.io/relatorios-educacionais-publicos-ruce/

Acessos diretos por aba:

- [Histórico de habilidades](https://diegofelipecorporativo-source.github.io/relatorios-educacionais-publicos-ruce/?painel=historico)
- [Comparativo por escola](https://diegofelipecorporativo-source.github.io/relatorios-educacionais-publicos-ruce/?painel=escolas)
- [Dispersão de estudantes](https://diegofelipecorporativo-source.github.io/relatorios-educacionais-publicos-ruce/?painel=dispersao)

## Cuidados com a publicação

O repositório é **público**: os relatórios HTML e os dados incorporados neles podem ser acessados por qualquer pessoa. Antes de enviar, confira se os arquivos não contêm dados pessoais identificáveis de estudantes, docentes, credenciais ou informações cujo compartilhamento não esteja autorizado.

Se os relatórios forem gerados novamente, basta substituir os três arquivos mantendo os mesmos nomes. Prefira arquivos HTML autossuficientes, com recursos internos ou caminhos relativos compatíveis com GitHub Pages. O portal não mistura dados entre as abas e não exige compactação dos HTMLs.
