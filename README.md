# IA de Triagem - Sistema Manchester

Sistema de inteligência artificial para triagem médica baseado no Protocolo de Manchester, classificando pacientes por urgência de atendimento.

# Níveis de Triagem
Cor	        Urgência	              Tempo Alvo
Vermelho	  Emergência Imediata	    0 minutos
Laranja	    Muito Urgente	          10 minutos
Amarelo	    Urgente	                60 minutos
Verde	      Pouco Urgente	          120 minutos
Azul	      Não Urgente	            240 minutos

Como Usar:
# Dados do paciente
paciente = {
    "queixa_principal": "Dor Torácica",
    "sinais_vitais": {"FC": 110, "PA_sistolica": 90, "SpO2": 92},
    "historico_paciente": {"idade": 65, "comorbidades": ["Hipertensão"]},
    "sintomas_adicionais": {"intensidade_dor": 8}
}

# Classificação
resultado = triagem_manchester(paciente)
print(f"Nível de triagem: {resultado}")  # Laranja

# Funcionalidades

   Avaliação automática baseada em sinais vitais e sintomas
   
   Classificação por cores conforme Protocolo Manchester
   
   Entrada flexível de dados do paciente
   
   Lógica hierárquica priorizando casos críticos

# Importante

Sistema de apoio à decisão clínica - não substitui avaliação médica profissional.
