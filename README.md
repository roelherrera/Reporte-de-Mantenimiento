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
