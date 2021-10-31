# MercadoLibre_Challenge
Challenge for Data Science interview at Mercadolibre 



# <font color='navy'><center>Evaluación Data Science</center></font>\

Se le asigna como tarea realizar un modelo que determine si un usuario de MercadoPago (MP) Argentina volverá a transaccionar en los próximos 2 meses. Para ello se cuenta con los siguientes archivos:\


* **PAYMENTS.csv:** Contiene datos transaccionales de MP que se hayan realizado en los últimos 6 meses. Este está sólo limitado al segmento Wallet (todos los pagos que se realicen con billetera virtual).
    * FECHA: Fecha en que se realizó exitosamente la transacción.
    * CUS_CUST_ID_SEL: ID del seller.
    * CUS_CUST_ID_BUY: ID del buyer.
    * SPENT: Dinero gastado en la transacción.
    * TPV_SEGMENT_DETAIL: Flujo que usó el usuario (Instore = QR, Transport = SUBE, Utilities = Pago de servicios, money transfer, Cellphone recharge).
    * DESCUENTO: Descuento que MP le otorgó en esa transacción.


* **ACTIVE_USER.csv:** Contiene datos de las visitas a la APP.
    * CUS_CUST_ID_BUY: ID del buyer.
    * MAU_MP_1: Cantidad de veces el usuario entró a la APP  de MP (azul) en el último mes de entrenamiento (mes -1).
    * MAU_ML_1: Cantidad de veces el usuario entró a la APP  de ML (amarilla) en el último mes de entrenamiento (mes -1).
    * MAU_ML_2: Cantidad de veces el usuario entró a la APP  de ML (amarilla) en el mes -2 de entrenamiento.
    * last_login_mp_date_1: Fecha del último login del mes en APP MP.


* **DEMOGRAFICOS.csv:** Contiene datos de la edad, sexo, tarjeta que usa y lugar de residencia.


* **DINERO_CUENTA.csv:** Contiene datos de la cantidad de dinero en la cuenta y si invierte en fondo.
    * PLATA_CUENTA_1: Máximo dinero en cuenta en el último mes (mes -1).
    * PLATA_CUENTA_2: Máximo dinero en cuenta en el mes -2.
    * INVERSION: Indica en que estado esta el usuario para la inversión:
        * Investing: Está invirtiendo.
        * Elegible: Está disponible para que inviertan dinero.
        * Warmup: Hicieron el onboarding de inversión pero no llenaron los campos.
        * Pending: Hicieron el proceso para invertir, pero está en pending de aprobación.


* **MARKETPLACE_DATA.csv:** Contiene un resumen a nivel usuario de movimientos en mercadolibre (ML) para los últimos 6 meses.
    * SPENT_ML: Dinero gastado en ML.
    * RECENCY_ML: Fecha de la ultimo compra en ML.
    * FREQUENCY_ML: Cantidad de días que realizó compras.
