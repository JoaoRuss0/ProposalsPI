<template>
    <b-container fluid>
        <b-row>
            <b-table class="m-5" :fields="fields" :items="items" hover head-variant="dark"></b-table>
        </b-row>
    </b-container>
</template>

<script>
export default {
    data() {
        return {
            fields: [
                {key: "numero", label: "Nº", sortable: true},
                {key: "designacao", label: "Designação/Tema" },
                {key: "modulos", label: "N.º módulos", sortable: true},
                {key: "areas", label: "Área temática", sortable: true},
                {key: "orientador", label: "Orientador", sortable: true},
                {key: "coorientadores", label: "Coorientadores", sortable: true},
                {key: "departamentos_coorientadores", label: "Departamentos Coorientadores" },
                {key: "Orientador(es) externos", label: "Orientador(es) externos", sortable: true},
                {key: "parcerias", label: "Parcerias", sortable: true},
                {key: "contactos", label: "Contacto(s)", sortable: true}
            ],
            items: [
                {
                    "numero": 1,
                    "designacao": "AmazFitBand@Autopsy",
                    "modulos": 1,
                    "areas": ["DA", "IF"],
                    "orientador": "Patrício Domingues",
                    "coorientadores": ["Miguel Frade"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 2,
                    "designacao": "Automatic Image Captioning for Forensics (AICF)",
                    "modulos": 1,
                    "areas": ["DA", "IF"],
                    "orientador": "Patrício Domingues",
                    "coorientadores": ["Miguel Frade", "Miguel Negrão"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 3,
                    "designacao": "MiHome@Autopsy",
                    "modulos": 1,
                    "areas": ["DA", "IF"],
                    "orientador": "Patrício Domingues",
                    "coorientadores": ["Miguel Frade", "Miguel Negrão"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 4,
                    "designacao": "Aplicação de Localização de Tags RFID Passivas em Ambientes Industriais",
                    "modulos": 4,
                    "areas": ["DA", "APD"],
                    "orientador": "João Pereira",
                    "coorientadores": ["Rui Vasco", "Sílvio Mendes"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 5,
                    "designacao": "Explorando o uso de técnicas de inteligência artificial na deteção de incidentes de segurança em redes IoT",
                    "modulos": 2,
                    "areas": ["SRC", "APD"],
                    "orientador": "Carlos Rabadão",
                    "coorientadores": ["Leonel Santos", "Rogério Costa"],
                    "departamentos_coorientadores": ["DEI", "CIIC"]
                },

                {
                    "numero": 6,
                    "designacao": "MOODoke: Emotion-based Karaoke",
                    "modulos": 1,
                    "areas": ["AED", "SM"],
                    "orientador": "Ricardo Malheiro"
                },

                {
                    "numero": 7,
                    "designacao": "Cibersegurança com recurso às Redes Neuronais Artificiais e um dispositivo SDR “Software Defined Radio”",
                    "modulos": 2,
                    "areas": ["DA", "APD"],
                    "orientador": "João Pereira",
                    "coorientadores": ["Humberto Ferreira"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 8,
                    "designacao": "Aplicação de Captura Automática de Ecrã por SDR “Software Defined Radio”",
                    "modulos": 1,
                    "areas": ["DA", "APD"],
                    "orientador": "João Pereira"
                },

                {
                    "numero": 9,
                    "designacao": "Redes Neuronais Artificiais em Deep Learning na deteção da doença COVID-19",
                    "modulos": 1,
                    "areas": ["DA", "APD"],
                    "orientador": "João Pereira"
                },

                {
                    "numero": 10,
                    "designacao": "Redes Neuronais Artificiais em Deep Learning na Modelação 3D de Edifícios",
                    "modulos": 1,
                    "areas": ["DA", "APD"],
                    "orientador": "João Pereira"
                },

                {
                    "numero": 11,
                    "designacao": "Redes Neuronais Artificiais em Deep Learning na Condução Autónoma de uma Cadeira de Rodas",
                    "modulos": 1,
                    "areas": ["DA", "APD"],
                    "orientador": "João Pereira"
                },

                {
                    "numero": 12,
                    "designacao": "NetworkMonit&Alarm",
                    "modulos": 1,
                    "areas": ["SOD", "SI"],
                    "orientador": "Carlos Antunes"
                },

                {
                    "numero": 13,
                    "designacao": "Device Tracking without GPS",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Carlos Antunes"
                },

                {
                    "numero": 14,
                    "designacao": "Cibersegurança para a Indústria 4.0",
                    "modulos": 2,
                    "areas": ["SRC", "APD"],
                    "orientador": "Carlos Rabadão",
                    "coorientadores": ["Leonel Santos", "Rogério Costa"],
                    "departamentos_coorientadores": ["DEI", "CIIC"]
                },

                {
                    "numero": 15,
                    "designacao": "Recriação Virtual da Cidade Romana de Miróbriga",
                    "modulos": 1,
                    "areas": ["CG", "SM"],
                    "orientador": "Alexandrino Gonçalves",
                    "coorientadores": ["Anabela Marto"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 16,
                    "designacao": "Gestão de Equipamentos Industriais",
                    "modulos": 1,
                    "areas": ["AWD"],
                    "orientador": "Marisa Maximiano",
                    "coorientadores": ["Francisco Santos"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 17,
                    "designacao": "Campus Maps",
                    "modulos": 2,
                    "areas": ["AWD", "CG", "DA"],
                    "orientador": "Nuno Veiga",
                    "coorientadores": ["Pedro Gago", "Anabela Marto"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 18,
                    "designacao": "SMA - Support Management Application",
                    "modulos": 2,
                    "areas": ["DA"],
                    "orientador": "Nuno Veiga",
                    "coorientadores": ["Ricardo Gomes"],
                    "departamentos_coorientadores": ["DEI"],
                    "orientadores_externos": ["Paulo Cruz"],
                    "parcerias": ["Ent.Externa (Devbrain)"]
                },

                {
                    "numero": 19,
                    "designacao": "Plataforma de gestão de sistemas de virtualização",
                    "modulos": 2,
                    "areas": ["RS"],
                    "orientador": "Nuno Veiga",
                    "coorientadores": ["Carlos Antunes"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 20,
                    "designacao": "Gestão de eventos de segurança",
                    "modulos": 2,
                    "areas": ["SRC"],
                    "orientador": "Nuno Veiga",
                    "coorientadores": ["Carlos Antunes"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 21,
                    "designacao": "Avaliação de sistemas de virtualização",
                    "modulos": 1,
                    "areas": ["RS"],
                    "orientador": "Nuno Veiga",
                    "coorientadores": ["Carlos Antunes"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 22,
                    "designacao": "Otimização de Processos de Picking IV",
                    "modulos": 1,
                    "areas": ["IA", "DA"],
                    "orientador": "Carlos Grilo",
                    "coorientadores": ["Luís Neves", "Eunice Oliveira"],
                    "departamentos_coorientadores": ["DEE", "DMAT"]
                }

                ,

                {
                    "numero": 23,
                    "designacao": "Desempenho de Redes Neuronais para sinais Unidimensionais",
                    "modulos": 1,
                    "areas": ["IA", "AC"],
                    "orientador": "Carlos Grilo",
                    "coorientadores": ["Luís Conde", "Mónica Figueiredo"],
                    "departamentos_coorientadores": ["DEE", "DEE"]
                },

                {
                    "numero": 24,
                    "designacao": "Defend Your Castle AR",
                    "modulos": 1,
                    "areas": ["CG", "SM"],
                    "orientador": "Anabela Marto",
                    "coorientadores": ["Alexandrino Gonçalves"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 25,
                    "designacao": "ATEMPHAR 2022",
                    "modulos": 2,
                    "areas": ["DA"],
                    "orientador": "Filipe Neves",
                    "coorientadores": ["Olga Craveiro"],
                    "departamentos_coorientadores": ["DEI"],
                    "parcerias": "Associação ATEMPHAR"
                },

                {
                    "numero": 26,
                    "designacao": "Distribuição e controlo inteligente de tarefas em ambiente de multicontrolador",
                    "modulos": 1,
                    "areas": ["SOD"],
                    "orientador": "António Pereira",
                    "coorientadores": ["João Ramos", "Nuno Costa"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 27,
                    "designacao": "Estação Meteorológica Móvel utilizando Drones",
                    "modulos": 1,
                    "areas": ["APD"],
                    "orientador": "João Ramos",
                    "coorientadores": ["António Pereira", "Luís Frazão"],
                    "departamentos_coorientadores": ["DEI","DEI"]
                },

                {
                    "numero": 28,
                    "designacao": "SABE4ELDERS – Serviço de Aquisição de Bens Essenciais para Idosos",
                    "modulos": 1,
                    "areas": ["RS", "AWD", "DA"],
                    "orientador": "David Safadinho",
                    "coorientadores": ["António Pereira"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 29,
                    "designacao": "Farm4All-IoT – Solução IoT para Agricultura Doméstica",
                    "modulos": 1,
                    "areas": ["RS", "APD", "DA"],
                    "orientador": "David Safadinho",
                    "coorientadores": ["Paulo Madeira"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 30,
                    "designacao": "aCreditar - Aplicação para gestão do processo de creditação",
                    "modulos": 1,
                    "areas": ["AWD", "AIBD"],
                    "orientador": "Pedro Gago",
                    "coorientadores": ["Vítor Távora", "Rui Brás"],
                    "departamentos_coorientadores": ["DEI", "DSI"]
                },

                {
                    "numero": 31,
                    "designacao": "Sistema inteligente para deteção de pessoas e incêndios utilizando Drones",
                    "modulos": 1,
                    "areas": ["IA"],
                    "orientador": "João Ramos",
                    "coorientadores": ["António Pereira", "Rolando Miragaia"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 32,
                    "designacao": "Mapeamento aéreo Inteligente 2D e 3D de Áreas Frutícolas utilizando Drones",
                    "modulos": 1,
                    "areas": ["APD", "IA"],
                    "orientador": "João Ramos",
                    "coorientadores": ["Rolando Miragaia", "António Pereira"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 33,
                    "designacao": "Veículos não tripulados na apanha inteligente de objetos usando visão computacional",
                    "modulos": 1,
                    "areas": ["APD", "IA"],
                    "orientador": "João Ramos",
                    "coorientadores": ["Rolando Miragaia", "António Pereira"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 34,
                    "designacao": "Aplicação Web para o CIIC - IPLeiria",
                    "modulos": 1,
                    "areas": ["AWD", "AIBD"],
                    "orientador": "Beatriz Piedade",
                    "coorientadores": ["Anabela Bernardino", "Eugénia Bernardino"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 35,
                    "designacao": "Soluções de Apoio à Condução de Viaturas",
                    "modulos": 2,
                    "areas": ["DA", "RS"],
                    "orientador": "Sílvio Mendes",
                    "coorientadores": ["Paulo Loureiro", "Paulo Costa"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 36,
                    "designacao": "Low Power Wide Area Networks 4 Smart Cities",
                    "modulos": 1,
                    "areas": ["GR","RC","RS"],
                    "orientador": "Luis Frazão",
                    "coorientadores": ["Daniel Fuentes", "Nuno Costa"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 37,
                    "designacao": "SmartLab IoT Controller",
                    "modulos": 1,
                    "areas": ["AWD","RS","SRC","APD"],
                    "orientador": "Luis Frazão",
                    "coorientadores": ["Daniel Fuentes"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 38,
                    "designacao": "Wi-Fi Security Analyzer",
                    "modulos": 1,
                    "areas": ["SRC"],
                    "orientador": "Luis Frazão",
                    "coorientadores": ["Daniel Fuentes"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 39,
                    "designacao": "IoT Security Operations",
                    "modulos": 1,
                    "areas": ["RS","SRC"],
                    "orientador": "Luis Frazão",
                    "coorientadores": ["Daniel Fuentes", "António Pereira"],
                    "departamentos_coorientadores": ["DEI","DEI"]
                },

                {
                    "numero": 40,
                    "designacao": "Sleeping Modes 4 IoT Power Saving",
                    "modulos": 1,
                    "areas": ["RS", "APD"],
                    "orientador": "Luis Frazão",
                    "coorientadores": ["David Safadinho", "António Pereira"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 41,
                    "designacao": "Aplicação para Rastreio de Viaturas",
                    "modulos": 2,
                    "areas": ["DA"],
                    "orientador": "Sílvio Mendes",
                    "coorientadores": ["Paulo Loureiro", "Paulo Costa"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 42,
                    "designacao": "Ecossistema de home-IoT inteligente para Active Ambient Assisted Living",
                    "modulos": 1,
                    "areas": ["SAD", "RS", "DA", "IA"],
                    "orientador": "António Pereira",
                    "coorientadores": ["Fernando Silva", "José Ribeiro"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 43,
                    "designacao": "Serviços de Dados para Sinais Rodoviários",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Sílvio Mendes",
                    "coorientadores": ["Paulo Loureiro", "Paulo Costa"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 44,
                    "designacao": "Inteligência Artificial para Classificação da Condução",
                    "modulos": 2,
                    "areas": ["DA", "IA"],
                    "orientador": "Sílvio Mendes",
                    "coorientadores": ["Paulo Loureiro", "Paulo Costa"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 45,
                    "designacao": "Receção e Apresentação de Informação de sinais de Transito em Aplicações",
                    "modulos": 2,
                    "areas": ["DA", "RA"],
                    "orientador": "Sílvio Mendes",
                    "coorientadores": ["Paulo Loureiro", "Paulo Costa"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 46,
                    "designacao": "WebOt - Uma plataforma Web para Problemas de Otimização",
                    "modulos": 1,
                    "areas": ["IA", "DAE"],
                    "orientador": "Carlos Grilo",
                    "coorientadores": ["Anabela Bernardino"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 47,
                    "designacao": "Vídeo porteiro low-cost (IoT)",
                    "modulos": 1,
                    "areas": ["GR", "RS"],
                    "orientador": "Paulo Madeira",
                    "coorientadores": ["David Safadinho"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 48,
                    "designacao": "Despertador low-cost (IoT)",
                    "modulos": 1,
                    "areas": ["GR", "RS"],
                    "orientador": "Paulo Madeira",
                    "coorientadores": ["David Safadinho"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 49,
                    "designacao": "Criação automática de datasets para machine learning",
                    "modulos": 1,
                    "areas": ["IA", "DA"],
                    "orientador": "Paulo Costa",
                    "coorientadores": ["Nuno Rodrigues"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 50,
                    "designacao": "Reconhecimento de Objetos 3D",
                    "modulos": 1,
                    "areas": ["IA", "DA"],
                    "orientador": "Paulo Costa",
                    "coorientadores": ["Nuno Rodrigues"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 51,
                    "designacao": "RPI Network Deployment",
                    "modulos": 1,
                    "areas": ["RS", "DA", "IOT"],
                    "orientador": "Daniel Fuentes",
                    "coorientadores": ["David Safadinho", "Luís Frazão"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 52,
                    "designacao": "Remote Desk Operator",
                    "modulos": 1,
                    "areas": ["GR", "RS", "DA", "IOT"],
                    "orientador": "Daniel Fuentes",
                    "coorientadores": ["Luís Frazão"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 53,
                    "designacao": "Edge Microservices in IoT with K8s",
                    "modulos": 1,
                    "areas": ["GR", "RS", "DA", "IOT"],
                    "orientador": "Daniel Fuentes",
                    "coorientadores": ["Luís Frazão"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 54,
                    "designacao": "Aero Clube de Leiria",
                    "modulos": 2,
                    "areas": ["AWD"],
                    "orientador": "Marco Monteiro"
                },

                {
                    "numero": 55,
                    "designacao": "Realidade Aumentada para monitorização e controlo de drones",
                    "modulos": 1,
                    "areas": ["RA", "DA"],
                    "orientador": "Nuno Rodrigues",
                    "coorientadores": ["Alexandrino Gonçalves", "Roberto Ribeiro"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 56,
                    "designacao": "Realidade Aumentada para formação e monitorização na indústria mineral",
                    "modulos": 1,
                    "areas": ["RA", "DA"],
                    "orientador": "Nuno Rodrigues",
                    "coorientadores": ["Roberto Ribeiro"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 57,
                    "designacao": "SAVVI – Spatial Awareness Vibration for the Visually Impaired",
                    "modulos": 1,
                    "areas": ["HCI", "TI", "DA", "GUR"],
                    "orientador": "Roberto Ribeiro",
                    "coorientadores": ["Nuno Rodrigues"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 58,
                    "designacao": "Face Detection and Emotion Recognition 4 AAL",
                    "modulos": 1,
                    "areas": ["ASI", "SAD", "APD"],
                    "orientador": "Roberto Ribeiro",
                    "coorientadores": ["José Ribeiro", "António Pereira"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 59,
                    "designacao": "Speech Emotion Recognition 4 AAL",
                    "modulos": 1,
                    "areas": ["ASI", "SAD", "APD"],
                    "orientador": "Roberto Ribeiro",
                    "coorientadores": ["José Ribeiro", "António Pereira"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 60,
                    "designacao": "MPoI – Marking real Points of Interest for the creation of virtual world",
                    "modulos": 1,
                    "areas": ["DA", "HCI"],
                    "orientador": "Roberto Ribeiro",
                    "coorientadores": ["Nuno Rodrigues"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 61,
                    "designacao": "Mecanismos de Inteligência Artificial para a Otimização da Performance de UAV",
                    "modulos": 1,
                    "areas": ["SAD", "DA", "IA"],
                    "orientador": "Fernando Silva",
                    "coorientadores": ["José Ribeiro", "Nuno Rodrigues", "Roberto Ribeiro"],
                    "departamentos_coorientadores": ["DEI", "DEI", "DEI"]
                },

                {
                    "numero": 62,
                    "designacao": "Social Plogging Lovers",
                    "modulos": 1,
                    "areas": ["AWD", "AIBD", "DA"],
                    "orientador": "Micaela Esteves",
                    "coorientadores": ["Rosa Matias", "Angela Pereira"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 63,
                    "designacao": "CeliAct",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Catarina Reis",
                    "coorientadores": ["Sónia Gonçalves Pereira", "Elga Ferreira"],
                    "departamentos_coorientadores": ["ciTechCare", "LiDA"]
                },

                {
                    "numero": 64,
                    "designacao": "MultiPrev 2.0",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Catarina Reis",
                    "coorientadores": ["Sónia Gonçalves Pereira"],
                    "departamentos_coorientadores": ["ciTechCare"]
                },

                {
                    "numero": 65,
                    "designacao": "RegulA 2.0",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Catarina Reis",
                    "coorientadores": ["Helena Reis", "Sara Simões Dias"],
                    "departamentos_coorientadores": ["ciTechCare", "ciTechCare"]
                },

                {
                    "numero": 66,
                    "designacao": "Implementação reduzida do standard IoT oneM2M",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Nuno Costa",
                    "coorientadores": ["Luis Frazão"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 67,
                    "designacao": "Cooperação Espontânea Centralizada entre Smart Objects via Standard IoT oneM2M",
                    "modulos": 2,
                    "areas": ["APD"],
                    "orientador": "Nuno Costa",
                    "coorientadores": ["Luis Frazão"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 68,
                    "designacao": "Cooperação Espontânea Distribuída entre Smart Objects via Standard IoT oneM2M",
                    "modulos": 2,
                    "areas": ["APD"],
                    "orientador": "Nuno Costa",
                    "coorientadores": ["Luis Frazão"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 69,
                    "designacao": "Aplicação para auxiilar pacientes em recuperação",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Olga Craveiro"
                },

                {
                    "numero": 70,
                    "designacao": "Art Evaluation using Depth Cameras to obtain Spectators’ Reactions",
                    "modulos": 1,
                    "areas": ["DA", "IA"],
                    "orientador": "Rolando Miragaia",
                    "coorientadores": ["José Ribeiro", "Gustavo Reis"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 71,
                    "designacao": "Evolutionary Art using Evolutionary Algorithms",
                    "modulos": 1,
                    "areas": ["SAD", "DA", "IA","SM"],
                    "orientador": "Rolando Miragaia",
                    "coorientadores": ["José Ribeiro", "Gustavo Reis"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 72,
                    "designacao": "Fruit ripeness analyses using deep learning models in natural environment",
                    "modulos": 1,
                    "areas": ["DA", "IA"],
                    "orientador": "Rolando Miragaia",
                    "coorientadores": ["Paulo Costa"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 73,
                    "designacao": "Respirar Fundo: Um sistema de apoio à atividade fisica",
                    "modulos": 1,
                    "areas": ["AWD", "AIBD", "DA"],
                    "orientador": "Micaela Esteves",
                    "coorientadores": ["Rosa Matias", "Angela Pereira", "Filipe Vieira"],
                    "departamentos_coorientadores": ["DEI", "DEI", "DEI"],
                    "parcerias": ["Sara Brito (Escola Secundária Rodrigues Lobo)"],
                    "contactos": ["Raul Antunes (ESECS)"]
                },

                {
                    "numero": 74,
                    "designacao": "Plataforma de gestão de Programas de Reabilitação Cardíaca",
                    "modulos": 2,
                    "areas": ["DA"],
                    "orientador": "Ricardo Martinho",
                    "coorientadores": ["Rui Rijo", "Rui Pinto"],
                    "departamentos_coorientadores": ["DEI", "DMAT"]
                },

                {
                    "numero": 75,
                    "designacao": "Aplicação web para gestão de estágios",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Vítor Távora",
                    "coorientadores": ["Rui Vasco Monteiro", "Eduardo Silva"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 76,
                    "designacao": "Aplicação web para calendário de avaliações",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Vítor Távora",
                    "coorientadores": ["Pedro Gago"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 77,
                    "designacao": "Aplicação Web para acompanhamento dos estudantes",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Vítor Távora",
                    "coorientadores": ["Pedro Gago"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 78,
                    "designacao": "Aplicação web para acompanhamento de ENE (2.0)",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Vítor Távora"
                },

                {
                    "numero": 79,
                    "designacao": "Aplicação web para distribuição do serviço docente",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Vítor Távora",
                    "coorientadores": ["Beatriz Piedade"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 80,
                    "designacao": "Community Health Monitor",
                    "modulos": 1,
                    "areas": ["AWD", "AIBD", "ACBD"],
                    "orientador": "Rosa Matias",
                    "coorientadores": ["Beatriz Piedade"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 81,
                    "designacao": "Portal Web - Experiências práticas na horta da escola no 1º ciclo",
                    "modulos": 1,
                    "areas": ["AWD"],
                    "orientador": "Eugénia Bernardino",
                    "coorientadores": ["Alexandrino Gonçalves", "Paula Mendes"],
                    "departamentos_coorientadores": ["DEI", "DEI"]
                },

                {
                    "numero": 82,
                    "designacao": "Plataforma para estimativas de projetos Salesforce",
                    "modulos": 1,
                    "areas": ["AWD", "AIBD", "DA"],
                    "orientador": "Sónia Luz",
                    "coorientadores": ["Marisa Maximiano"],
                    "departamentos_coorientadores": ["DEI"],
                    "parcerias": ["Merkle"],
                    "contactos": ["Ana Catarina Brites, Salesforce Managing Consultant"]
                },

                {
                    "numero": 83,
                    "designacao": "Programa de Fidelidade",
                    "modulos": 1,
                    "areas": ["AWD"],
                    "orientador": "Sónia Luz",
                    "coorientadores": ["Marisa Maximiano"],
                    "departamentos_coorientadores": ["DEI"],
                    "parcerias": ["Merkle"],
                    "contactos": ["Dário Santos, Practice Lead Paulo Reis, Lead Consultant"]
                },

                {
                    "numero": 84,
                    "designacao": "Aplicação web para Inscrição nos Turnos",
                    "modulos": 1,
                    "areas": ["DA"],
                    "orientador": "Vítor Távora",
                    "coorientadores": ["Pedro Gago"],
                    "departamentos_coorientadores": ["DEI"]
                },

                {
                    "numero": 85,
                    "designacao": "Aplicação web para gestão da UC Projeto Informático",
                    "modulos": 2,
                    "areas": ["DA"],
                    "orientador": "Vítor Távora",
                    "coorientadores": ["Sónia Luz"],
                    "departamentos_coorientadores": ["DEI"]
                }
            ]
        }
    }
}
</script>

<style>
* {
    font-family: "Segoe UI" !important;
    font-size: small !important;
}

table {
    border-collapse: separate !important;
    border-spacing: 0 !important;
}

th {
    border: 0px !important;
    vertical-align: middle !important;
}

tr td:first-child{
    border-left: 1px solid #dee2e6 !important;
}

tr td:last-child{
    border-right: 1px solid #dee2e6 !important;
}

table tr:last-child td {
    border-bottom: 1px solid #dee2e6 !important;
}

/* top-left border-radius */
table tr:first-child th:first-child {
    border-top-left-radius: 10px !important;
}

/* top-right border-radius */
table tr:first-child th:last-child {
    border-top-right-radius: 10px !important;
}

/* bottom-left border-radius */
table tr:last-child td:first-child {
    border-bottom-left-radius: 10px !important;
}

/* bottom-right border-radius */
table tr:last-child td:last-child {
    border-bottom-right-radius: 10px !important;
}
</style>
