# Deploy de Aplicação Utilizando Container no Cloud Run

## Cloud Run 
Ele é um serviço gerenciado do <b>Google Cloud Platform (GCP)</b> que permite executar aplicativos em contêineres de forma escalável. Com o Cloud Run, você pode <i>implantar facilmente seus <b>contêineres Docker</b></i> em um ambiente totalmente gerenciado, sem se preocupar com a configuração de servidores ou dimensionamento da infraestrutura.

A <b>principal característica</b> do Cloud Run é sua capacidade de dimensionamento automático. Isso significa que o serviço <i>ajusta automaticamente</i> o número de instâncias do contêiner com base na carga de tráfego recebida. Se houver um <b>aumento</b> repentino no tráfego, o Cloud Run criará mais instâncias para lidar com a demanda. Por outro lado, se o tráfego diminuir, ele <b>reduzirá</b> o número de instâncias para economizar recursos.

Ao utilizar o Cloud Run, você pode se beneficiar das seguintes vantagens:

<table>
	<ol>
		<li><b>Escalabilidade automática:</b> O Cloud Run escala horizontalmente suas aplicações com base na demanda, permitindo que você atenda a picos de tráfego sem problemas. Você só paga pelas instâncias em execução, o que o torna econômico.</li>
		<li><b>Flexibilidade:</b> O Cloud Run suporta contêineres do Docker, permitindo que você use a linguagem de programação, as bibliotecas e as estruturas de sua escolha para desenvolver suas aplicações. Você pode aproveitar as vantagens do ecossistema do Docker para construir e compartilhar imagens de contêineres.</li>
		<li><b>Integração com o ecossistema do GCP:</b> O Cloud Run se integra perfeitamente com outros serviços do Google Cloud Platform. Você pode usar o Cloud Build para automatizar o processo de construção e implantação de contêineres, o Cloud Logging para monitorar logs e o Cloud Monitoring para acompanhar o desempenho da aplicação.</li>
		<li><b>Implantação rápida:</b> O Cloud Run permite que você faça o deploy de suas aplicações de forma rápida e simples. Com apenas alguns comandos ou cliques no console do GCP, você pode disponibilizar sua aplicação para uso imediato.</li>
		<li><b>Compatibilidade com padrões do setor:</b> O Cloud Run é construído com base no padrão Knative, que oferece um conjunto de APIs e componentes para desenvolvimento e execução de aplicações em contêineres. Isso garante a portabilidade das suas aplicações e facilita a migração para outras plataformas que suportam o padrão Knative.</li>
	</ol>
</table>

