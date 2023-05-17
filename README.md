# Deploy de Aplicação Utilizando Container no Cloud Run

## Cloud Run 
Ele é um serviço gerenciado do <b>Google Cloud Platform (GCP)</b> que permite executar aplicativos em contêineres de forma escalável. Com o Cloud Run, você pode <i>implantar facilmente seus <b>contêineres Docker</b></i> em um ambiente totalmente gerenciado, sem se preocupar com a configuração de servidores ou dimensionamento da infraestrutura.

A <b>principal característica</b> do Cloud Run é sua capacidade de dimensionamento automático. Isso significa que o serviço <i>ajusta automaticamente</i> o número de instâncias do contêiner com base na carga de tráfego recebida. Se houver um <b>aumento</b> repentino no tráfego, o Cloud Run criará mais instâncias para lidar com a demanda. Por outro lado, se o tráfego diminuir, ele <b>reduzirá</b> o número de instâncias para economizar recursos.

Ao utilizar o Cloud Run, você pode se beneficiar das seguintes vantagens:

<table>
	<ol>
		<li><b>Escalabilidade automática:</b> O Cloud Run escala horizontalmente suas aplicações com base na demanda, permitindo que você atenda a picos de tráfego sem problemas. Você só paga pelas instâncias em execução, o que o torna econômico.</li>
		<br>
		<li><b>Flexibilidade:</b> O Cloud Run suporta contêineres do Docker, permitindo que você use a linguagem de programação, as bibliotecas e as estruturas de sua escolha para desenvolver suas aplicações. Você pode aproveitar as vantagens do ecossistema do Docker para construir e compartilhar imagens de contêineres.</li>
		<br>
		<li><b>Integração com o ecossistema do GCP:</b> O Cloud Run se integra perfeitamente com outros serviços do Google Cloud Platform. Você pode usar o Cloud Build para automatizar o processo de construção e implantação de contêineres, o Cloud Logging para monitorar logs e o Cloud Monitoring para acompanhar o desempenho da aplicação.</li>
		<br>
		<li><b>Implantação rápida:</b> O Cloud Run permite que você faça o deploy de suas aplicações de forma rápida e simples. Com apenas alguns comandos ou cliques no console do GCP, você pode disponibilizar sua aplicação para uso imediato.</li>
		<br>
		<li><b>Compatibilidade com padrões do setor:</b> O Cloud Run é construído com base no padrão Knative, que oferece um conjunto de APIs e componentes para desenvolvimento e execução de aplicações em contêineres. Isso garante a portabilidade das suas aplicações e facilita a migração para outras plataformas que suportam o padrão Knative.</li>
	</ol>
</table>

Para fazer o deploy de uma aplicação utilizando contêineres no Cloud Run, deve fazer o seguinte:

<table>
	<ol>
		<li><b>Containerização da aplicação:</b> Primeiro, você precisa containerizar sua aplicação usando o Docker. Isso envolve escrever um arquivo Dockerfile que define a configuração necessária para executar sua aplicação em um contêiner. O Dockerfile especifica as dependências, comandos de construção e configurações do ambiente de execução.</li>
		<br>
		<li><b>Construção e envio do contêiner:</b> Após escrever o Dockerfile, você deve construir a imagem do contêiner usando o comando docker build. Certifique-se de ter o Docker instalado em sua máquina. Em seguida, envie a imagem do contêiner para o Container Registry do GCP usando o comando <code>docker push</code></li>.
		<br>
		<li><b>Criação do serviço do Cloud Run:</b> No Console do GCP, vá para o Cloud Run e crie um novo serviço. Forneça um nome e selecione a região em que deseja implantar o serviço. Escolha a opção "Implantar um contêiner" e selecione a imagem do contêiner que você enviou para o Container Registry.</li>
		<br>
		<li><b>Configuração do serviço:</b> Na configuração do serviço do Cloud Run, você pode definir várias opções, como a quantidade de memória e a quantidade máxima de instâncias do contêiner. Também é possível configurar variáveis de ambiente, definir a exposição de portas e configurar gatilhos de eventos.</li>
		<br>
		<li>Implantação do serviço: Após configurar todas as opções necessárias, clique em "Implantar" para implantar o serviço do Cloud Run. O GCP provisionará automaticamente os recursos necessários e iniciará o contêiner da sua aplicação.</li>
		<br>
		<li>Acesso à aplicação: Após a implantação bem-sucedida, o Cloud Run fornecerá um URL público para acessar a sua aplicação. Você pode usar esse URL para acessar e testar a aplicação.</li>
	</ol>
</table>