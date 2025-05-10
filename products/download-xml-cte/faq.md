# D�vidas Frequentes

**1. Os XMLs baixados pela funcionalidade possuem validade jur�dica?** <br>
Sim, o XML de CT-e baixado possu� validade jur�dica, pois s�o baixados diretamente da Sefaz.

**2. A funcionalidade baixa os XML desde quando a empresa come�ou a emitir CT-e?** <br>
N�o, a Sefaz s� permite que sejam baixados os XML emitidos nos �ltimos 90 dias. Sendo assim, esse � o limite da funcionalidade.

**3. A funcionalidade de CT-e est� configurada corretamente e estava funcionado, mas parou de baixar os XMLs. E o CT-e consta no portal da Sefaz. O que pode ser?** <br>
O processo de integra��o entre a Sefaz estadual e a Sefaz nacional pode estar com problema. Com isso n�o � poss�vel efetuar os downloads. Para verificar isso, entre no portal da Sefaz nacional e consulte um CT-e n�o est� conseguindo baixar (pela chave). No Box _�SITUA��O ATUAL :AUTORIZADO�_ observe a coluna _�Data Recebimento AN�_ se estiver preenchido com uma data inv�lida, como _�01/01/0001 � 00:00:00�_ significa que a integra��o entre Sefaz estadual e a Sefaz nacional est� com problemas.
Exemplo
_Exemplo_

![imagem-problema-sefaz-cte](./imagens/problema-sefaz-cte.jpg)

_Nesses casos voc� deve entrar em contato com a Sefaz de seu estado para que o servi�o seja normalizado_

**4 � A Sefaz fornece algum lugar para verificar a disponibilidade dos servi�os de download de NF-e ou CT-e?** <br>
N�o, at� o momento n�o existe um local onde possa ver a disponibilidade desses servi�os, desse modo as vezes os servi�os podem estar inoperantes e n�o ter por onde monitorar.

**5 � Aparece o seguinte erro no console ao tentar efetuar o download:�Value=�A WSDL exception occurred at0:0 WsdlParser Exception :Error sending SOAP message:Peer certificate cannot be authenticated with given CA certificates�** <br>
Esse erro geralmente � referente aos arquivos do certificado digital do cliente. Execute o processo descrito nos links abaixo para sanar o problema. <br>
> [-> Link 01 do TDN](https://centraldeatendimento.totvs.com/hc/pt-br/articles/360022658731-Cross-Segmento-TOTVS-Backoffice-Linha-Protheus-ADVPL-Peer-certificate-cannot-be-authenticated-with-given-CA-certificates) <br>
> [-> Link 02 do TDN](https://tdn.totvs.com/pages/viewpage.action?pageId=223932805) <br>
> [-> Link 03 do TDN](https://tdn.totvs.com/display/tec/Acesso+a+Web+Services+que+exigem+certificados+de+CA) <br>

**6 � Estou tendo as seguintes rejei��es ao tentar efetuar o download:** <br>
�641 � Rejei��o:NF-e indisponivel para o emitente� <br>
-> �640 � Rejei��o:CNPJ/CPF do interessado n�o possui permiss�o para consultar esta NF-e� <br>
-> As rotinas fazem download das CT-e das quais o cnpj da empresa � o destinat�rio ou tomador. Caso esteja tentando efetuar o download de notas que pr�ria empresa emitiu (de sa�da), ou notas emitidas para um CNPJ diferente ao da empresa, isso n�o ser� poss�vel.

