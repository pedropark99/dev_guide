

## Versão de lançamento do livro <inserir versão>

### Manutenção do repositório entre lançamentos

- [ ] Consulte as páginas de *issues* dos repositórios do GitHub [do guia do desenvolvedor](https://github.com/ropensci/dev_guide/issues), e [da meta de revisão de software](https://github.com/ropensci/software-review -meta/issues), para descobrir quais são as alterações que ainda estão para serem feitas no guia do desenvolvedor. Atribua esses problemas/*issues* do guia de desenvolvimento à *milestones* (ou "marcos") cadastrados no repositório do GitHub, que são correspondentes às versões que você está lançando. Seja tanto para a próxima versão, ou, a seguinte, por exemplo, a [versão 0.3.0](https://github.com/ropensci/dev_guide/milestone/2). Incentive os PRs (*pull requests*), e faça com que eles sejam revisados.



### 1 mês antes do lançamento

- [ ] Lembre os editores de abrir problemas/PRs para itens (ou *features*) que eles desejam ver na próxima versão.

- [ ] Execute [a função `devguide_prerelease()`](https://github.com/ropensci-org/devguider) do pacote `devguider`.

- [ ] Peça aos editores qualquer feedback que você precise deles antes do lançamento.

- [ ] Para cada contribuição/alteração verifique se o campo NOTÍCIAS no `Apêndice.Rmd` foi atualizado.

- [ ] Planeje uma data para o lançamento em comunicação com o gerente da comunidade do rOpenSci, que lhe dará uma data para publicar uma postagem no blog (ou nota técnica).


### 2 semanas antes do lançamento

- [ ] Escreva um rascunho para um blog post (ou uma nota técnica) que conta sobre o lançamento. Escreva esse rascunho com antecedência o suficiente para que tanto os editores quanto, em seguida, o gerente da comunidade, possam revisá-lo (2 semanas).
[Exemplo](https://github.com/ropensci/roweb3/pull/291), [instruções gerais para postagem no blog](https://blogguide.ropensci.org/), [instruções específicas para postagens de lançamento](#releaseblogpost ).

- [ ] Faça um PR a partir de uma branch `dev` para a branch `master`, e, avise os editores no GitHub e Slack. Mencione em algum comentário dentro deste PR o rascunho que você escreveu para o blog post (ou a nota técnica).



### Hora do lançamento

- [] Verifique todas as URLs usando [a função `devguide_urls()` do pacote {devguider}](https://github.com/ropensci-org/devguider)

- [] Verifique a ortografia usando [a função `devguide_spelling()` do pacote {devguider}](https://github.com/rpensci-org/devguider). Atualize a [WORDLIST](https://github.com/ropensci/dev_guide/blob/master/inst/WORDLIST) conforme necessário.

- [ ] Caso necessário, faça um squash sobre os seus commits, e, em seguida, mescle o PR da branch `dev` para a branch `master`.

- [ ] Crie a Release (ou `lançamento`) no GitHub, e verifique o lançamento do Zenodo.

- [ ] Reconstrua manualmente o livro (para atualização dos metadados do Zenodo no livro), ou então, aguarde a compilação diária que é realizada no repositório.

- [] Recrie a branch de desenvolvimento (`dev`).

- [ ] Termine o seu blog post (ou nota técnica) no PR. Ao longo da discussão do PR, também reforçe os aspectos mais importantes a serem destacados nos tweets de divulgação.
