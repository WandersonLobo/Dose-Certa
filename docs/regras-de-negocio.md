# Regras de negócio

### Usuários e autorizações

| ID | Regra de negócio |
| --- | --- |
| RN01 | Todo usuário deverá atuar como paciente, cuidador ou ambos simultaneamente. |
| RN02 | Um paciente poderá autorizar múltiplos cuidadores, assim como um cuidador poderá acompanhar múltiplos pacientes. |
| RN03 | A autorização concedida a um cuidador deverá abranger todos os tratamentos do respectivo paciente. |
| RN04 | A revogação de uma autorização deverá impedir novos acessos e operações do cuidador sobre os dados do paciente, preservando os registros anteriormente realizados. |

### Medicamentos

| ID | Regra de negócio |
| --- | --- |
| RN05 | O catálogo de medicamentos deverá ser compartilhado entre os usuários, sendo cada medicamento diferenciado pela combinação de nome, concentração e forma farmacêutica. |

### Tratamentos e prescrições

| ID | Regra de negócio |
| --- | --- |
| RN06 | Um paciente poderá possuir zero ou mais tratamentos, e cada tratamento deverá pertencer obrigatoriamente a exatamente um paciente. |
| RN07 | Um tratamento poderá possuir duração determinada ou indeterminada. |
| RN08 | Um tratamento deverá possuir uma ou mais prescrições, e cada prescrição deverá pertencer obrigatoriamente a exatamente um tratamento. |
| RN09 | Uma prescrição deverá possuir um ou mais itens prescritos, e cada item prescrito deverá pertencer a exatamente uma prescrição. |
| RN10 | Um medicamento poderá estar associado a diferentes prescrições e poderá aparecer mais de uma vez em uma mesma prescrição, desde que possua orientações distintas. |
| RN11 | Cada item prescrito deverá estar associado a exatamente um medicamento do catálogo. |
| RN12 | Somente o paciente ou um cuidador autorizado poderá registrar prescrições e alterações nas orientações referentes aos tratamentos do paciente. |

### Orientações prescritas

| ID | Regra de negócio |
| --- | --- |
| RN13 | Cada item prescrito deverá possuir suas próprias orientações de dosagem, frequência, horários e período de utilização. |
| RN14 | O período de utilização de cada item prescrito poderá ser independente dos demais, desde que respeite os limites temporais do tratamento. |
| RN15 | Um item prescrito somente poderá possuir período de utilização indeterminado quando estiver associado a um tratamento de duração indeterminada. |
| RN16 | As alterações nas orientações prescritas deverão preservar as orientações anteriores e identificar o usuário responsável pelo registro. |
| RN17 | Uma alteração nas orientações prescritas deverá possuir data e horário de início de vigência iguais ou posteriores ao momento de seu registro, conforme a orientação recebida. |

### Estados dos tratamentos

| ID | Regra de negócio |
| --- | --- |
| RN18 | Um tratamento deverá possuir um dos seguintes estados: em andamento, interrompido ou concluído. |
| RN19 | A interrupção de um tratamento deverá registrar a data, o motivo e o usuário responsável pelo registro. |
| RN20 | Um tratamento poderá ser concluído manualmente ou automaticamente ao atingir sua data de término. A interrupção ou conclusão deverá cancelar as doses futuras ainda não administradas, preservando seus registros. |

### Doses e administrações

| ID | Regra de negócio |
| --- | --- |
| RN21 | Cada dose programada deverá estar associada à orientação prescrita que originou sua programação. |
| RN22 | As alterações nas orientações prescritas deverão atualizar ou cancelar as doses futuras afetadas, preservando as doses passadas, as administrações registradas e o histórico das orientações. |
| RN23 | Uma dose deverá possuir um dos seguintes estados: pendente, administrada, esquecida, administrada com atraso ou cancelada. |
| RN24 | Somente o paciente ou um cuidador autorizado poderá registrar a administração de uma dose não cancelada. |
| RN25 | Cada administração deverá registrar a data e o horário reais da utilização do medicamento, bem como o usuário responsável pelo registro. |
| RN26 | Uma dose pendente deverá ser considerada esquecida quando ultrapassar 24 horas após seu horário programado sem administração registrada. |
| RN27 | Uma dose anteriormente identificada como esquecida poderá ter sua administração registrada posteriormente. |
| RN28 | A classificação de uma dose administrada deverá considerar o horário real da administração, independentemente do momento do registro, sendo considerada atrasada quando administrada após o horário programado. |
| RN29 | Uma dose poderá possuir, no máximo, um registro de administração. |

### Lembretes

| ID | Regra de negócio |
| --- | --- |
| RN30 | Cada lembrete deverá estar associado a exatamente uma dose programada. |
| RN31 | Os lembretes deverão ser destinados ao paciente e não deverão ser emitidos para doses canceladas ou que já possuam administração registrada. |

### Limites de atuação do sistema

| ID | Regra de negócio |
| --- | --- |
| RN32 | O sistema possui caráter exclusivamente organizacional e informativo, não devendo realizar diagnósticos, prescrições, recomendações de medicamentos ou alterações autônomas nas orientações estabelecidas pelos profissionais de saúde. |
