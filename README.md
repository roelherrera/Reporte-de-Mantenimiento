# Reporte-de-Mantenimiento
Reporte Necesidades Mantenimiento en ABAP (SAP R/3)

*&---------------------------------------------------------------------*
*& Report  YPMR0021
*&
*&---------------------------------------------------------------------*
*& Proyecto...: X                                                      *
*& Módulo.....: PM                                                     *
*& Funcional..: Roel Herrera                                           *
*& Transacción: YPMR021                                                *
*& Autor......: Roel Herrera                                           *
*& Fecha......: 31.08.2018                                             *
*& Descripción: Reporte Necesidades Mantenimiento                      *
*&---------------------------------------------------------------------*
*& MODIFICACIONES                                                      *
*&---------------------------------------------------------------------*
*& Funcional..: Roel Herrera                                           *
*& Autor......: Roel Herrera                                           *
*& Fecha......: 13.11.2018                                             *
*& Id/REN...  : PE-20181016                                            *
*& Motivo.....: No considerar Avisos con status exclusivo MECE         *
*& Marca......: @001                                                   *
*&---------------------------------------------------------------------*

REPORT  YPMR0021.

INCLUDE YPMR0021_TOP.   "Global data
INCLUDE YPMR0021_SEL.   "Selection Screen
INCLUDE YPMR0021_CLA.   "Class Implementation
INCLUDE YPMR0021_MAI.   "Main Program

---------------------------------------------------------------------

Textos de Selección
C_MECE	Restringir Avisos MECE
P_DWERK	Centro
P_LAYOUT	Layout
S_ERDAT	Fecha de Entrada

---------------------------------------------------------------------

Símbolos de Texto
001	PENDIENTE
002	CERRADA
003	PROGRAMADA
011	Estado
021	Desc.Aviso
022	Descripción Aviso
023	Descripción de Aviso
031	Den.Equipo
032	Den.Equipo
033	Denominación Equipo
041	A.I.Plan.
042	Act.Int.Plan.
043	Costo Act.Int.Plan.
051	A.E.Plan.
052	Apr.Ext.Plan.
053	Costo Apr.Ext.Plan.
061	M.P.Plan.
062	Mat.Pro.Plan.
063	Costo Mat.Pro.Plan.
071	AI+AE+MP P
072	AI+AE+MP Plan.
073	Costo ActInt+AprExt+MatPro Planificados
081	A.I.Real
082	Act.Int.Real
083	Costo Act.Int.Real
091	A.E.Real
092	Apr.Ext.Real
093	Costo Apr.Ext.Real
101	M.P.Real
102	Mat.Pro.Real
103	Costo Mat.Pro.Real
111	AI+AE+MP R
112	AI+AE+MP Reales
113	Costo ActInt+AprExt+MatPro Reales
121	F.Cre.Avi.
122	Fe.Cre.Aviso
123	Fe.Creación Aviso
131	OT
132	Num.OT
133	Número OT
141	Tip.OT
142	Tipo OT
143	Tipo OT
151	Fe.Plan.
152	Fecha Plan.
153	Fecha Planificación
161	Fe.Plan.
162	Fecha Plan.
163	Fecha Planificación
171	Fe.Prog.
172	Fecha Prog.
173	Fecha Programación
181	Actividad
191	Resp.
192	Responsable
201	Solic.
202	Solicitante
211	Condición
221	Costo Plan
222	Costo Planificado
231	Costo Real
241	A.E+MP P
242	ActExt+MatPro Plan.
243	Act.Ext+Mat.Pro.Planificados
251	A.E+MP R
252	ActExt+MatPro Real
253	Act.Ext+Mat.Pro.Reales
B01	Parámetros de Selección
B02	Selección de Layout
B03	Parámetros de Restricción
C01	N° Avisos Pendientes
C02	Número de Avisos Pendientes
C03	N° Avisos Programados
C04	Número de Avisos Programados
C05	N° Avisos Cerrados
C06	Número de Avisos Cerrados
C07	Total
C08	Cumplimiento
CO1	QMNUM
CO2	AUFNR
ST1	STATUS
T01	Reporte Necesidades Mantenimiento
