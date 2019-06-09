# Yandex Object Storage

Just add service provider for yandex cloud

## Install

Via composer:

    composer require flipe23/yandex-object-storage-provider

## Usage

After installing this package add the following code to your config/filesystems.php:

    'yandex' => [
                'driver' => 'yandexcloud',
                'key' => 'your-key',
                'secret' => 'your-secret',
                'bucket' => 'bucket-name',
                'region' => 'us-east-1',
    ],
    
And then you can use

    $disk = Storage::disk('yandex');

to get your yandex cloud storage instance

###### Don't forget to add the Flipe23\YandexObjectStorage\YandexObjectStorageProvider to your $providers array if your laravel version lower than 5.5