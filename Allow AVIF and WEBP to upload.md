function allow_modern_images( $mime_types ) {
 $mime_types['heic'] = 'image/heic';
 $mime_types['heif'] = 'image/heif';
 $mime_types['heics'] = 'image/heic-sequence';
 $mime_types['heifs'] = 'image/heif-sequence';
 $mime_types['avif'] = 'image/avif';
 $mime_types['avifs'] = 'image/avif-sequence';
 $mime_types['svg'] = 'image/svg+xml';
 $mime_types['svgz'] = 'image/svg+xml';
 return $mime_types;
}
add_filter( 'upload_mimes', 'allow_modern_images');
