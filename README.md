CAN_SALDO_CUOTAS_APLICADO numeric(21,9) SI Saldo de la cuenta en cuotas despues de aplicado
el movimiento
COD_AGENCIA varchar(5) SI Identificador de Agencia
COD_CUENTA varchar(15) SI Identificador unico de Cuenta Individual
perteneciente a un afiliado o de Cuenta Colectiva
de un patrono dentro del sistema. Las cuentas
pertenecen a los clientes. Las cuentas se
almacenan en la tabla FO.FO_CUENTAS
COD_EMPRESA varchar(5) NO Identificador de Empresa
COD_INVERSION varchar(5) SI Identificador del Fondo de Inversion
COD_SISTEMA varchar(2) SI Codigo de sistema o modulo de P2000 que
identifica el registro, el cual puede afectar un
permiso, dependencia o ambito de un parametro
dentro del sistema. Se parametriza en la tabla
PA.SISTEMAS
COD_TIPSALDO varchar(4) SI Identificador del saldo.
DESCRIPCION varchar(80) SI Descripcion del movimiento. Se toma de la
descripcion del catalogo PA.SUBTIP_TRANSAC
Campo Tipo dato Nulo Descripción
de PA
ESTADO char(1) SI Codigo de estado actual que identifica el registro,
el cual puede afectar un proceso. un calculo o un
resultado. Los valores posibles para este campo
pueden ser: "P" Pendiente, "A" Aplicado
FEC_APLICADO datetime SI Fecha de aplicacion del movimiento
FEC_INCLUSION datetime SI Auditoria: Fecha en que se incluyo el registro
FEC_MODIFICACION datetime SI Auditoria: Fecha en que se modifico el registro por
ultima vez
FEC_MOVIMTO datetime NO Fecha del movimiento.
FEC_MOVIMTO_DETA datetime SI Fecha del movimiento detalle.
FEC_REZAGO datetime SI Fecha de registro del rezago
FORMA_PAGO varchar(5) SI Forma de pago EFE:Efectivo, CKL:Cheque Local,
CKE:Cheque Extranjero
HORA_MOVIMTO datetime SI Hora del movimiento
INCLUIDO_POR varchar(10) SI Auditoria: Identificador de Usuario que incluyo
registro
MODIFICADO_POR varchar(10) SI Auditoria: Usuario que modifico el registro por
ultima vez
MON_MOVIMTO numeric(21,9) SI Monto del movimiento
MON_SALDO_APLICADO numeric(21,9) SI Saldo de la cuenta despues de aplicado el
movimiento
NUM_MOVIMTO numeric(12,0) NO Numero del movimiento.
NUM_MOVIMTO_DETA numeric(12,0) NO Numero del movimiento del detalle.
NUM_PAT varchar(20) SI Numero patronal
NUM_REZAGO varchar(6) SI Número de rezago
OBSERVACIONES varchar(500) SI Observaciones del movimiento
REF_SCR varchar(20) SI Referencia SICERE
SUBTIP_TRANSAC varchar(5) SI Codigo de Movimiento detalle o Subtransaccion
que identifica el registro a nivel de movimientos o
parametros. El catalogo se obtiene de la tabla
PA.SUBTIP_TRANSAC en el Modulo de PA
(Politicas Administrativas).
TIP_MOVIMTO char(1) SI Tipo de movimiento. Los posibles valores son: "D"
Debito, "C" Credito, "N" Ninguno
TIP_TRANSAC numeric(3,0) SI Codigo de Movimiento o Transaccion que
identifica el registro a nivel de movimientos o
parametros. El catalogo se obtiene de la tabla
Diseño de Estructura
PA.TIP_TRANSAC en el Modulo de PA (Politicas
Administrativas).
TOT_CUOTA numeric(21,9) SI Total de cuotas del movimietno.
TRANSAC_SICERE varchar(5) SI Codigo del movimiento original enviado por
SICERE en el archivo de recaudacion
VALOR_CUOTA numeric(21,9) SI Monto del valor cuota con que se compraron las
cuotas
