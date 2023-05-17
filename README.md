# Deploy de Aplicação Utilizando Container no Cloud Run

## Cloud Run 
Ele é um serviço gerenciado do <b>Google Cloud Platform (GCP)</b> que permite executar aplicativos em contêineres de forma escalável. Com o Cloud Run, você pode <i>implantar facilmente seus <b>contêineres Docker</b></i> em um ambiente totalmente gerenciado, sem se preocupar com a configuração de servidores ou dimensionamento da infraestrutura.

A <b>principal característica</b> do Cloud Run é sua capacidade de dimensionamento automático. Isso significa que o serviço <i>ajusta automaticamente</i> o número de instâncias do contêiner com base na carga de tráfego recebida. Se houver um <b>aumento</b> repentino no tráfego, o Cloud Run criará mais instâncias para lidar com a demanda. Por outro lado, se o tráfego diminuir, ele <b>reduzirá</b> o número de instâncias para economizar recursos.