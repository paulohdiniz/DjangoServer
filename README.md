<ol type="1">
	<li>Cria pasta do projeto</li>
	<li>Verifica qual variavel do python (se é py3, python, python3 etc), pip (pip ou pip3) e se virtualenv está ok (pipx list).</li>
	<li> Se o virtualenv não estiver instalado e verifica depois com pipx list.
		pipx install virtualenv
		<code>
			OBS: Esse pipx é pra indicar que é pip ou pip3.

			OBS: Eu evitei instalar o virtualenvwrapper-win porque quando tentei deu muito
			problema.

			OBS:	python -m pip install openpyxl  é equivalente a pip install openpyxl. 
			Algumas pessoas preferem a primeira forma como garantia de qual versão do pip 
			será executada e onde os módulos serão instalados.
		</code>
	</li>
	<li>Cria o virtual env.
		virtualenv NOMEDAENV 
	</li>
	<li>Abra o PowerShell como ADM e coloca:
		Set-ExecutionPolicy RemoteSigned
		autoriza com um SIM. (Isso permite com que vc consiga ativar o script activate)
	</li>
	<li>vá até a pasta NOMEDAENV>Scripts> e digita:
			.\activate
		Aqui vc estará dentro da sua virtualenv, aparecerá ela no terminal 
		entre parenteses (NOMEDAENV).
		OBS: para desativar basta digitar "deactivate" em qualquer lugar 
		que vc sairá da virtualenv.
	</li>
	<li>Agora você instala o django e outras dependencias que quiser para o seu projeto.
		pipx install -r requirements.txt (caso tenha)
		pipx install django
		OBS: sempre verifique se foi instalado vendo a versão (p ex: django-admin --version) ou dando um pipx list.
	</li>
	<li> Criando um servidor teste:
		django-admin startproject nomeDoMeuSite
	</li>
	<li>Ligando o servidor.
		Entra na pasta nomeDoMeuSite e executa:
		python3 manage.py runserver
	</li>
	<li>Jogue http://127.0.0.1:8000/ no seu navegador e veja se está tudo ok !</li>
	<li>Criando e salvando as dependencias:
		pipx freeze > requirements.txt
	</li>
	<li>Git ignore.

		Se seu ambiente virtual está dentro da pasta venv por exemplo, 
		adicione venv/ no .gitignore

		OBS: Há arquivos bem completos de gitignore ja prontos na web, segue um link:
		https://github.com/github/gitignore/blob/master/Python.gitignore
	</li>
	<li></li>

</ol>


6) 

7) 



8)

9) 

10) 

11) 
12) 