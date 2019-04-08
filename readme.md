# Yandex Object Storage

Just add service provider for yandex cloud

## Usage

---

After installing this package add the following code to your config/filesystems.php:

    'yandex' => [
                'driver' => 'yandexcloud',
                'key' => 'your-key',
                'secret' => 'your-secret',
                'bucket' => 'bucket-name',
    ],

And then you can use

    $disk = Storage::disk('yandex');

to get your yandex cloud storage instance

###### Don't forget to add the Flipe23\YandexObjectStorage\YandexObjectStorageProvider to your $providers array if your laravel version lower than 5.5