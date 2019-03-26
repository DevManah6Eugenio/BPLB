# BPLB
Impressora de etiquetas ELGIN L-42

Etiqueta

N (limpa o buffer de impressão)<br>
D13 (configura a Densidade ou aquecimento da cabeça de impressão)<br>
S1 (configura a velocidade de impressão 1 polegadas/segundo)<br>
JF (habilita o “backfeed” para que ao final da impressão, o espaço entre etiquetas pare na serrilha)<br>
ZT (indica que a impressão deve iniciar a partir do topo)<br>
A170,40,0,4,1,2,N,"<EMPRESA>" (campo de texto)<br>
A25,110,0,3,1,1,N,"NF-e: @numero" (campo de texto)<br>
A25,140,0,3,1,1,N,"Remetente: @remetente" (campo de texto)<br>
A25,170,0,3,1,1,N,"Destinatario: @destinatario" (campo de texto)<br>
A25,200,0,3,1,1,N,"Volumes: @quant @vols Peso: @peso CT-e @ctrc" (campo de texto)<br>
A300,270,0,4,1,1,N,"@cid_dest-@uf_dest" (campo de texto)<br>
P1 (indica a quantidade de etiquetas que serão impressas, nesse caso 1)<br>
