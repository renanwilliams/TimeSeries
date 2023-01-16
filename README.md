# TimeSeries - PredictingPopulationNYCMetro

Banco de dados do metrô de Nova York. Descrição dos campos anexada abaixo.

O objetivo principal é prever o número de pessoas que usam o metrô. Você pode deixar a imaginação trabalhar e fazer da forma que preferir, escolhendo a taxa de amostragem temporal/espacial (por estação/catraca, dia/hora/semana etc).

DESCRIÇÃO DOS CAMPOS:

CA,UNIT,SCP,STATION,LINENAME,DIVISION,DATE,TIME,DESC,ENTRIES,EXITS

CA = Área de controle (A002); UNIT = Unidade remota para uma estação (R051); SCP = Subunidade A posição do canal representa um endereço específico para um dispositivo (02-00-00); STATION = Representa o nome da estação em que o dispositivo está localizado; LINENAME = Representa todas as linhas de trem que podem ser embarcadas nesta estação. Normalmente as linhas são representadas por um caractere. LINENAME 456NQR representa o servidor de trem para os trens 4, 5, 6, N, Q e R.; DIVISION = Representa a Linha originalmente a estação pertencia a BMT, IRT ou IND; DATE = Representa a data (MM-DD-YY); TIME = Representa a hora (hhmmss) para um evento de auditoria agendado; DESC = Representa o evento de auditoria REGULAR agendado ( Normalmente ocorre a cada 4 horas) 1. As auditorias podem ocorrer por mais de 4 horas devido a atividades de planejamento ou solução de problemas. 2. Além disso, pode haver uma entrada RECOVR AUD Refere-se a uma auditoria perdida que foi recuperada.; ENTRIES = O valor do registro de entrada comulativo para um dispositivo; EXITS = O valor cumulativo do registro de saída para um dispositivo.

Exemplo:
Os dados abaixo mostram os valores do registro de entrada/saída para uma catraca na área de controle (A002) de 092714 às 00:00 horas a 092914 às 00:00 horas.

CA,UNIT,SCP,STATION,LINENAME,DIVISION,DATE,TIME,DESC,ENTRIES,EXITS A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,000000,REGULAR,0004800073,0001629137, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,040000,REGULAR,0004800125,0001629149, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,080000,REGULAR,0004800146,0001629162, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,120000,REGULAR,0004800264,0001629264, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,160000,REGULAR,0004800523,0001629328, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,200000,REGULAR,0004800924,0001629371, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,000000,REGULAR,0004801104,0001629395, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,040000,REGULAR,0004801149,0001629402, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,080000,REGULAR,0004801168,0001629414, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,120000,REGULAR,0004801304,0001629463, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,160000,REGULAR,0004801463,0001629521, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,200000,REGULAR,0004801737,0001629555, A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-29-14,000000,REGULAR,0004801836,0001629574,


