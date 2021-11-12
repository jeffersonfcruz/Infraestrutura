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
			Desabilitar a Busca DNS
			
			BANNER MOTD #""#
			Mensagem de inicialização do Dispositivo

			ENABLE SECRET (senha)
			Define uma senha para entrar em modo de execução
		
			USERNAME (usuario) SECRET (senha)
			Define um Usuario e uma senha de Criptografia Tipo-5
		
			USERNAME (usuario) PASSWORD (senha)
			Define um Usuario e uma senha de Criptografia Tipo-7
		
			INTERFACE (Porta)
			entra em modo de configuração da interface (rede)
			
			IP DOMAIN-NAME (nome do dominio.X)
			Define um nome para o Dominio
		
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
		    
		    		DESCRIPTION (Descrição:)
		    		Informa uma Breve Descrição da Porta que irá ser Configurada
		    
		    		IP ADRESS (IP + SUB MASK)
		    		Configurar IP e Máscara de Rede para o dispositivo
				
				-/-
				
				LINE VTY (Quantidade de Linhas que será Disponivel (0,15)
				As linhas vty permitem acesso a um dispositivo Cisco via Telnet
				
				TRANSPORT INPUT ALL
				Permite todos os protocolos disponiveis para conexões de entrada para o seu roteador/switchs
				
				IP DEFAULT-GATEWAY (IP do roteador/Gateway)
				Define um IP (Gateway) para o Roteador
				
				INTERFACE VLAN 1
				Entra em Modo de Configuração de VLAN
				
				NO SHUTDOWN
				Ativa uma Interface/VLAN/Porta
				
				CRYPTO KEY GENERATE RSA GENERAL-KEYS MODULUS 1024
				> http://deptal.estgp.pt:9090/cisco/ccna1/course/module11/11.2.4.4/11.2.4.4.html
				
				IP SSH VERSION 2
				Altera a versão do Protocolo SSH
				
				IP SSH TIME-OUT (segundos)
				Define um tempo limite para o Protocolo SSH
				
	END
	Voltar diretamente ao modo de execução

	EXIT
	Sair e voltar ao Ultimo nivel

	CTRL+Z
	Sai da configuração global

	COPY RUNNING-CONFIG STARTUP-CONFIG
	Salva as Configurações
		
	SHOW IP INTERFACE BRIEF
	Mostra os IPs Configurados para a Interface
	SHOW VLAN BRIEF
	Mostra os IPs Configurados para a as VLANs
	
