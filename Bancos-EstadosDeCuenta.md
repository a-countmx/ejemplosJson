# Consumo de Timbrado Estados de Cuenta :bellhop_bell:

Este es un ejemplo para el consumo del servicio de timbrado enfocado a Estados de cuentas bancarios  :

Para el uso adecuado de los endpoint favor de acceder aquí :

https://documenter.getpostman.com/view/2417533/UVyn1dXE




## Ejemplo de Json para estados de cuenta :star:

```json
{
 "serie": "",
 "folio": 2,
 "fecha": "2022-11-17T14:00:32",
 "formaDePago": "04",
 "CondicionesDePago": "",
 "subtotal": 0.01,
 "descuento": 0.01,
 "total": 0.00,
 "moneda": "MXN", 
 "tipoDeComprobante": "I",
 "metodoPago": "PUE",
 "lugarExpedicion": "44950",
 "rfcEmisor": "JES900109Q90",
 "nombreEmisor": "JIMENEZ ESTRADA SALAS",
 "regimenFiscaEmisor": "601",
 "rfcReceptor": "MOHR8509137AA",
 "nombreReceptor": "RUBEN MORA HIGA TAMASHIRO",
 "usoCFDIReceptor": "S01",
 "domicilioCPReceptor": "45170",
 "regimenFiscalReceptor": "621", 
 "conceptoDetalles": [
   {
    "objetoImp": "02",
     "claveProdServ": "84121500",
     "claveUnidad": "E48",       
     "cantidad": 1,
     "unidad": "UNIDAD DE SERVICIO",     
     "descripcion": "SERVICIOS BANCARIOS",
     "valorUnitario": 0.01,
     "importe": 0.01,          
     "descuento": 0.01,          
     "impuestosTraslados": [
       {
         "base": 0.01,
         "impuesto": "002",
         "tipoFactor": "Tasa",
         "tasaOCuota": 0.00,
         "importe": 0.00
       }
     ]
   }
 ],
 "trasladosFactura": [
   {
     "base": 0.01,
     "impuesto": "002",
     "tipoFactor": "Tasa",
     "tasaOCuota": 0.00,
     "importe": 0.00
   }
 ]
}
```



## Datos a considerar :mag:

Estos serian prácticamente los datos que tendriamos que cambiar en nuestro caso :



*  **serie** : Serie
*  **folio** : Folio consecutivo
*  **fecha** : Fecha de emisión (puede regresarse la fecha hasta 72horas para atrás, pero no se puede adelantar)



*  **lugarExpedicion** :  lugar de expedición de la institución bancaria
*  **rfcEmisor** : Rfc de la institución bancaria
*  **nombreEmisor**  : Nombre de la institución bancaria
*  **regimenFiscaEmisor** : Régimen Fiscal de la institución bancaria



*  **rfcReceptor** :  RFC del cliente
*  **nombreReceptor** : Nombre del cliente
*  **domicilioCPReceptor** : Código postal del cliente
*  **regimenFiscalReceptor** : Régimen Fiscal 

