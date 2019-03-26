# BPLB
Impressora de etiquetas ELGIN L-42

Etiqueta

N (limpa o buffer de impressão)<br>
D13 (configura a Densidade ou aquecimento da cabeça de impressão)
S1 (configura a velocidade de impressão 1 polegadas/segundo)
JF (habilita o “backfeed” para que ao final da impressão, o espaço entre etiquetas pare na serrilha)
ZT (indica que a impressão deve iniciar a partir do topo)
A170,40,0,4,1,2,N,"<EMPRESA>" (campo de texto)
A25,110,0,3,1,1,N,"NF-e: @numero" (campo de texto)
A25,140,0,3,1,1,N,"Remetente: @remetente" (campo de texto)
A25,170,0,3,1,1,N,"Destinatario: @destinatario" (campo de texto)
A25,200,0,3,1,1,N,"Volumes: @quant @vols Peso: @peso CT-e @ctrc" (campo de texto)
A300,270,0,4,1,1,N,"@cid_dest-@uf_dest" (campo de texto)
P1 (indica a quantidade de etiquetas que serão impressas, nesse caso 1)
