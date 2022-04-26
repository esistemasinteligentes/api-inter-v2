# CONSULTAR SALDO-INTER

## Consultar Saldo
Para trazer o saldo da conta

```php
    $dd = new stdClass;
    $dd->certificate = '../cert/Inter_API_Certificado.crt';
    $dd->certificateKey = '../cert/Inter_API_Chave.key';
    $dd->client_id = '';//seu client_id
    $dd->client_secret = '';//client_secret
    $dd->data = '';

    
    $bankingInter = new InterBanking($dd);

    echo "<pre>";
    $saldo = $bankingInter->checkSaldo('');
    print_r($saldo);
```