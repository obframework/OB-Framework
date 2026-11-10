# ob_utillitruck (Enhanced)

Adaptacao do [smoke_utillitruck 1.0.3](https://github.com/BigSmoKe07/smoke_utillitruck)
para a OB Framework. Modelo e codigo originais: BigSmoKe07 e PNWParksFan.
Licenca GPL-3.0 preservada em `LICENSE`. Codigo adaptado sem `ox_lib`.

Spawn code: `utillitruck4` (nao substitui o `utillitruck` original do GTA).
Entre como motorista, pressione H para baixar os pes estabilizadores e use
as setas para subir/descer ou girar a cesta. Ao apertar H novamente, a cesta
desce e gira gradualmente ate a posicao de repouso; o caminhao fica freado
ate o fim desse recolhimento. A colisao
invisivel da cesta e criada localmente para cada jogador proximo. O servidor
valida que quem controla e o motorista e publica as animacoes nas statebags;
o cliente nao grava nelas, compativel com `sv_stateBagStrictMode true`.
Se o motorista sair com a cesta levantada, a posicao fica registrada para o
proximo motorista continuar o recolhimento antes de dirigir.

Os arquivos `.yft` e `.ytd` desta copia foram convertidos para Enhanced pelo
Alchemist CLI 1.0.0.56 e ficam exclusivamente em `stream_enhanced/`.
`v_boomtruck.ycd` foi copiado sem alteracao pelo conversor. Os arquivos Legacy
originais continuam em `stream/` dentro de
`corerp2/resources/[cars]/ob_utillitruck`; o download original nao foi alterado.

O `server.cfg` inicia `[cars]`. Para testar sem reiniciar o servidor, use
`refresh` e `ensure ob_utillitruck`, depois `/car utillitruck4` e teste com
outro jogador observando a cesta. Conversao de arquivo e validacao estatica
nao substituem esse teste em jogo, sobretudo da animacao `.ycd` na Enhanced.
