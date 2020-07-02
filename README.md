# Projeto Fonte de Tensão
  Projeto da disciplina Elêtronica para Computação (SSC0180-2020101) 2020, USP São Carlos.
O projeto consiste no desenvolvimento e simulação de uma fonte de tensão que converta a corrente alternada da tomada de tensão 110V ou de 220V  para uma tensão ajustável de 3V a 12V de corrente contínua com capacidade de 100mA.

# Simulação da fonte no Falstad

- ## Diagrama

![Diagrama Falstad](https://user-images.githubusercontent.com/50035537/85894871-ee270480-b7cb-11ea-880a-54c6f959e943.png)


 - ## Componentes utilizados
 
 	- Capacitor: Estabilização da tensão no circuito por meio do armazenamento de quantidades de energia.
	
	- Ponte de Diodos: Aproveitar os dois ciclos da tensão (Ajuda na transformação da corrente alternada vinda da tomada em corrente contínua no circuito).
	
	- Diodo Zener: Limitar a tensão que passa pelo circuito, estabelecendo uma tensão limite.
	
	- Potênciometro: Resistor em que é possível ajustar sua resistência.
	
	- Resistor: Limitar a corrente elétrica em um circuito.
	
	- Switch: Permitir a passagem de corrente elétrica para o circuito, funcionando como uma chave de liga e desliga.
	
	- Transistor NPN: Regula a corrente de coletor a partir da corrente de base, na qual a corrente de coletor é 100x a corrente de base.
	
	- Transformador: Converter a Tensão de 110V ou de 220V da tomada para 20V no circuito.
	
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
| Transformador | (110V / 220V) / 1.2A / 12V + 12V | [35.00 R$](https://produto.mercadolivre.com.br/MLB-791922427-transformador-1212-12a-trafo-1200ma-12v-12v-ac-12a-trafo-_JM?quantity=1) | 1 |

**Custo Total**: 49.00 R$.

 - ## Justificativa para escolha dos componentes

	- Transformador: Suporta uma corrente de 1.2A, e a corrente mínima que deve suportar no circuito é de aproximadamente 420mA.
	
	- Ponte de Diodos 2W10: Aguenta uma tensão de até 1000 V e bloqueia uma corrente de até 2 Amperes.
	
	- Capacitor de 470µF: Aguenta uma tensão de até 25V, sendo que a tensão máxima nessa parte do circuito é de aproximadamente 21V.
	
	- Resistor de 470Ω: Limita a corrente que passa pelo diodo zener. Aguenta uma potência de até 0.25W, sendo o mínimo necessário de aproximadamente 0.13W.
	
	- Resistor de 390Ω: Limitar a tensão da saída em no mínimo 3V, podendo assim colocar o potênciometro em resitência máxima. Aguenta uma potência de 0.25W, sendo o mínimo necessário aproximadamente 0.12W.
	
	- Diodo Zener 13V: Limita a tensão em 13V. Dessa forma, como ao passar pelo transistor há uma perda de 0.7V a saída terá uma tensão de no máximo 12.3V. Assim, para a saída ter exatos 12V, o potênciometro não necessita ser colocado em sua mínima resistência.
	
	- Transistor NPN: Aguenta 60V de tensão e suporta 800mA de corrente, sendo que a corrente máxima que passará por ele é de 100mA.
	
	- Potênciometro de 1KΩ: Suporta uma potência de 0.20W, e no circuito tem que suportar 0.13W. Regula a corrente que vai para a base do transistor NPN, permitindo que na saída tenha uma variação de 3V ~ 12V e 24.5mA ~ 100mA.
  
- ## Link para o circuito no falstad
  http://tinyurl.com/yboz8xpa
- ## Link para o vídeo explicativo:
  https://www.youtube.com/watch?v=hgTtiHER5eE&feature=youtu.be
# Projeto do Esquemático e do PCB no EAGLE

- ## Esquemático
  ![Esquemático Eagle](https://user-images.githubusercontent.com/50035537/85894919-039c2e80-b7cc-11ea-94b1-561e1887bce7.jpeg)


- ## PCB
  ![PCB](https://user-images.githubusercontent.com/50035537/85894935-0b5bd300-b7cc-11ea-9720-afdfa974d3c0.jpeg)

# Participantes

 - João Antônio Misson Milhorim. Número USP: 18834331.
 - João Victor Sene Araújo. Número USP: 11796382.
 - Vitor Caetano Brustolin. Número USP: 11795589.
