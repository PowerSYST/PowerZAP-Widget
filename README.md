Bem-vindo a documentação do Widget PowerZAP.

O Widget possibilita a personalização de todos os elementos disponíveis no mesmo, para isto veja abaixo os métodos disponíveis. Execute os métodos do widget após o carregamento do mesmo.

##Parâmetros

###Objeto com parâmetros iniciais do Widget PowerZAP
```
$_PowerZAP = {};
```

###Carregar após o carregamento do Widget
```
$_PowerZAP.afterLoad = function(chat, box) { }
```

chat = instância do obejto PowerZAP
box  = elemento do box do PowerZAP

###Idioma do widget (pt-bt or en):
```
$_PowerZAP.lang = “pt-br”;
```

###Cor do botão de iniciar o box:
```
$_PowerZAP.color_btn = “#FF09098”;
```

###Texto quando o atendimento estiver online:
```
$_PowerZAP.textOnline = “Atendimento online”;
```

###Texto quando o atendimento estiver offline:
```
$_PowerZAP.textOffline = “Atendimento offline”;
```

###Domínio para armazena a sessão cookie:
```
$_PowerZAP.domain = “example.com.br”;
```

###Mensagem inicial:
```
$_PowerZAP.messageInitial = “Texto inicial da conversa”;
```

##Métodos

###Edite os dados iniciais do formulário:
```
PowerZAP.setData(name, whatsapp, department);
```

###Finalize o chat:
```
PowerZAP.closeChat();
```

###Abra o box do chat:
```
PowerZAP.openChat();
```

##Exemplo de Uso:
```
<script>
	$_PowerZAP = {
        color_btn : '#FF09098',
        afterLoad : function(chat, box_chat) {
            chat.setData('Exemplo nome', '5500999999999');
        },
        lang: 'pt-br'
    };
</script>
<!--- SCRIPT DO SEU WIDGET DISPONÍVEL NO PAINEL //-->
```