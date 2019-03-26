# BPLB
Etiqueta criada para impressora de etiquetas ELGIN L-42

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

<h2>- Comando "A"</h2>
  comando "A" representa a entrada de texto, como sera demostrado abaixo<br>

Sintaxe: Ap1，p2， p3，p4，p5，p6，p7，＂DADOS＂<br>
p1：Coordenada X em pontos (8 pontos = 1mm)<br>
p2：Coordenada Y em pontos (8 pontos = 1mm)<br>
p3：Rotação de impressão, escala： 0～3<br>
p4： Identificador da fonte a ser impressa，escala： 1～5， A～Z<br>
p5： Multilplica de 1 a 8 vezes na horizontal<br>
p6：Multilplica de 1 a 8 vezes na vertical<br>
p7： Reverso ou Não， N： não-reverso， R： reverso<br> 
DADOS： Dados a serem impressos<br>
