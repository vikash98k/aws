# aws
## ADD IN installation app --- >  'storages'

AWS_ACCESS_KEY_ID = config('AWS_ACCESS_KEY_ID')

AWS_SECRET_ACCESS_KEY = config('AWS_SECRET_ACCESS_KEY')

AWS_STORAGE_BUCKET_NAME = config('AWS_STORAGE_BUCKET_NAME')


AWS_S3_FILE_OVERWRITE = False

AWS_DEFAULT_ACL = None
# pip install django-storages
# pip install boto3
# configuration in installed app 'storages'
# CORS[(https://docs.aws.amazon.com/AmazonS3/latest/userguide/ManageCorsUsing.html#cors-example-1)]
STATICFILES_STORAGE = 'storages.backends.s3boto3.S3StaticStorage'
DEFAULT_FILE_STORAGE = "storages.backends.s3boto3.S3Boto3Storage"
