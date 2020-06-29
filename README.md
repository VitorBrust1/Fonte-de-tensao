# Projeto Fonte de Tensão
  Projeto da disciplina Elêtronica para Computação (SSC0180-2020101) 2020, USP São Carlos.
O projeto consiste no desenvolvimento e simulação de uma fonte de tensão que converta a corrente alternada da tomada de tensão 127V  para uma tensão ajustável de 3V a 12V de corrente contínua com capacidade de 100mA.

# Simulação da fonte no Falstad

- ## Diagrama

![Diagrama Falstad](https://user-images.githubusercontent.com/50035537/85894871-ee270480-b7cb-11ea-880a-54c6f959e943.png)


 - ## Componentes utilizados
 
 	- Capacitor: Estabilização da tensão no circuito por meio do armazenamento de quantidades de energia.
	
	- Ponte de Diodos: Aproveitar os dois ciclos da tensão (Ajuda na transformação da corrente alternada vinda da tomada em corrente contínua no circuito).
	
	- Diodo Zener: Limitar a tensão que passa pelo circuito.
	
	- Potênciometro: Resistor em que é possível ajustar sua potência.
	
	- Resistor: Limitar a corrente elétrica em um circuito.
	
	- Switch: Permitir a passagem de corrente elétrica para o circuito, funcionando como uma chave de liga e desliga.
	
	- Transistor NPN: Regula a corrente de coletor a partir da corrente de base, na qual a corrente de coletor é 100x a corrente de base.
	
	- Transformador: Converter a Tensão de 127V da tomada para 20V no circuito.
	
 - ## Preços e especificações
 
| Nome | Especificações | Preço(unidade) | Quantidade |
|--|--|--|--|
| Capacitor | 470µF / 25V | [0.33 R$](https://www.baudaeletronica.com.br/capacitor-eletrolitico-470uf-25v.html) | 1 |
| Ponte de Diodo 2W10 | 1000V / 2A | [0.90 R$](https://produto.mercadolivre.com.br/MLB-1425220046-20pcs-diodo-2w10-2a-1000v-ponte-retificadora-queima-de-estoq-_JM?quantity=1#position=2&type=item&tracking_id=7da9028e-051c-4f32-9131-fbebcf4951f3) | 1 |
| Diodo Zener | 13V / 0.1A | [1.06 R$](https://produto.mercadolivre.com.br/MLB-911630639-10-pcs-diodo-zener-13v-1w-1n4743frete-brasil-r1200-_JM?quantity=1#position=1&type=item&tracking_id=04c09c17-2e4c-4791-8f42-f5dba14f20db) | 1 |
| Potênciometro | 1KΩ / 0.2W | [1.23 R$](https://www.baudaeletronica.com.br/potenciometro-linear-rotativo-de-1k-1000.html) | 1 |
| Resistor | 390Ω / 0.25W | [0.12 R$](https://produto.mercadolivre.com.br/MLB-873476711-resistor-390-ohms-14w-5-kit-100-pcs-_JM?quantity=1#position=21&type=item&tracking_id=bb601283-825f-405d-88d3-7b98e6115a90) | 1 |
| Resistor | 470Ω / 0.25W | [0.86 R$](https://produto.mercadolivre.com.br/MLB-868726201-kit-10-x-resistor-470-ohm-5-14w-025w-leds-5mm-arduino-pic-_JM?quantity=1#position=3&type=item&tracking_id=47bb88f9-93a7-404e-95fa-2983eb8989df) | 1 |
| Switch | 250V / 6A | [8.90 R$](https://produto.mercadolivre.com.br/MLB-1273705844-chave-gangorra-redonda-on-off-spst-_JM?quantity=1#position=17&type=item&tracking_id=b7cc1b9b-29d5-4e13-a0b3-b4ef4f160cbb) | 1 |
| Transistor NPN | 60V / 0.8A | [0.60 R$](https://produto.mercadolivre.com.br/MLB-1222136291-20-pecas-transistor-npn-2n2222a-_JM?quantity=1#position=1&type=item&tracking_id=a8cdd5b8-c51f-44e9-a07f-8d04e5635adc) | 1 |	
| Transformador | 127V / 220V | [76.00 R$](https://www.viewtech.ind.br/catalog/product/view/id/3972/s/autotransformador-500va-110v-220v-bivolt/?utm_source=&utm_medium=&utm_campaign=&utm_term=&utm_content=&gclid=Cj0KCQjwoub3BRC6ARIsABGhnybLfUtYToxigt_hA1BKP5rDfu7k-AI21gttJaz3zLrME670AAGzHXwaAu6QEALw_wcB) | 1 |

 - ## Justificativa para escolha dos componentes

	- Transformador: Tensão de 127V
	
	- Ponte de Diodos 2W10: Aguenta uma tensão de até 1000 V e bloqueia uma corrente de até 2 Amperes.
	
	- Capacitor de 470µF: Aguenta uma tensão de 25V, sendo que o mínimo necessario pro circuito é de aproximadamente 21V.
	
	- Resistor de 470Ω: Aguenta uma potência de até 0.25W, sendo que o mínimo necessário para o circuito é de aproximadamente 0.13W. Ele tem por função diminuir a corrente que passará pelo diodo zener. 
	
	- Resistor de 390Ω: Aguenta uma potência de até 0.25W, sendo que o mínimo necessário para o circuito é de aproximadamente 0.13W. Ele tem por função , junto ao potênciometro, limitar a tensão de saída do circuito entre 3V e 12V.
	
	- Diodo Zener 13V: Aguenta uma tensão de 13V. Ele tem por função limitar a tensão no circuito em até 13V.
	
	- Transistor NPN: Aguenta 60V e 0.8A, sendo que a corrente máxima que passará por ele é de 0.1A e uma tensão máxima de 8.4V.
	
	- Potênciometro de 1KΩ: Aguenta uma potência de 0.2W, e o circuito necessita de um potênciomentro que aguente 0.1W. Permite a regulagem da quantidade de tensão (3V a 12V) na saída do circuito.
  
- ## Link para o circuito no falstad
  http://tinyurl.com/yboz8xpa
- ## Link para o vídeo explicativo:
  https://www.youtube.com/channel/UCYX2BrasfmQPxD01NNn-ICA?view_as=subscriber

# Projeto do Esquemático e do PCB no EAGLE

- ## Esquemático
  ![Esquemático Eagle](https://user-images.githubusercontent.com/50035537/85894919-039c2e80-b7cc-11ea-94b1-561e1887bce7.jpeg)


- ## PCB
  ![PCB](https://user-images.githubusercontent.com/50035537/85894935-0b5bd300-b7cc-11ea-9720-afdfa974d3c0.jpeg)

# Participantes

 - João Antônio Misson Milhorim. Número USP: 18834331.
 - João Victor Sene Araújo. Número USP: 11796382.
 - Vitor Caetano Brustolin. Número USP: 11795589.
