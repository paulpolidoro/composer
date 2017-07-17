# paulpolidoro/mask

Para criação de máscaras de CPF, CEP, Monetária, Telefone, etc

Composer install
Instalação via composer


```
composer require paulpolidoro/mask
```

or add on your composer.json file
ou adicionar no seu arquivo composer.json


How to use
Como usar


Applying default masks
Aplicando mascaras pré definidas


```php
// Formatando CEP
echo Mask::create(88888888, Mask::MASK_CEP);
// 88888-888

// Formatando TELEFONE
echo Mask::create(8888888888, Mask::MASK_TEL10);
// (88) 8888-8888

// Formatando CELULAR (9 dígitos)
echo Mask::create(888888888, Mask::MASK_TEL11);
// (88) 88888-8888
```

Creating custom masks
=====================
Criando mascaras personalizadas
===============================
```php
echo Mask::create(8888888888, "##.###-####.#");
// 88.888-8888.8

echo Mask::create(88888888, "##/##/##-##);
// 88/88/88-88
```
