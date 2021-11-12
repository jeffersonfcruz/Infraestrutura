# Infraestrutura
Estudo sobre Infraestrutura de Redes
## Comandos para configuração de roteadores e switchs CISCO

        ENABLE
	    Habilitar o modo de Execução
    DISABLE
    Desabilita o modo de Execução
	            
            CONFIGURE TERMINAL
	    Habilitar o Modo de configuração Global
	            	            
            HOSTNAME (nome do dispositivo)
	    Altera o nome do dispositivo    

            SERVICE PASSWORD-ENCRYPTION
	    Criptografa a Senha
                
            NO IP DOMAIN-LOOKUP
	    
	    BANNER MOTD #""#
	    Mensagem de inicialização do Dispositivo
                
            ENABLE SECRET (senha)
            Define uma senha para entrar em modo de execução

            USERNAME (usuario) SECRET (senha)
            Define um Usuario e uma senha de Criptografia Tipo-5

            USERNAME (usuario) PASSWORD (senha)
            Define um Usuario e uma senha de Criptografia Tipo-7

            LINE CONSOLE 0
            entrar em nivel configuração da porta console
			    
            LOGIN LOCAL
            Forçar a Fazer Autenticação com Logins Locais do Switch
	    
	    LOGGING SYNCHRONOUS
	    Sincronizar as Mensagens de Log na Tela			
	    
	    PASSWORD
	    define uma senha de Criptografia 
	    EXEC-TIMEOUT ()
	    Definir um Tempo de Sessão

            INTERFACE (Porta)
	    entra em modo de configuração da interface (rede)
	    
	    	DESCRIPTION Interface de Gateway da LAN
                Informa uma Breve Descrição da Porta que irá ser Configurada

                IP ADRESS (IP + SUB MASK)
		Configurar IP e Máscara de Rede para o dispositivo
				
    END
    Voltar ao modo de execução Diretamente
    
    EXIT
    Sair e voltar ao Ultimo nivel
    
    CTRL+Z 
	Sai da configuração global

    COPY RUNNING-CONFIG STARTUP-CONFIG
	Salva as Configurações