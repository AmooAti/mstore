WebP Express 0.15.3. Conversion triggered using bulk conversion, 2019-09-24 05:49:06

*WebP Convert 2.1.4*  ignited.
- PHP version: 7.3.1
- Server software: Apache

Stack converter ignited

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2017/02/beetroot-quinoa2.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/02/beetroot-quinoa2.jpg.webp
- log-call-arguments: true
- converters: (array of 9 items)

The following options have not been explicitly set, so using the following defaults:
- converter-options: (empty array)
- shuffle: false
- preferred-converters: (empty array)
- extra-converters: (empty array)

The following options were supplied and are passed on to the converters in the stack:
- default-quality: 70
- encoding: "auto"
- max-quality: 80
- metadata: "none"
- near-lossless: 60
- quality: "auto"
------------


*Trying: cwebp* 

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2017/02/beetroot-quinoa2.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/02/beetroot-quinoa2.jpg.webp
- default-quality: 70
- encoding: "auto"
- low-memory: true
- log-call-arguments: true
- max-quality: 80
- metadata: "none"
- method: 6
- near-lossless: 60
- quality: "auto"
- use-nice: true
- command-line-options: ""
- try-common-system-paths: true
- try-supplied-binary-for-os: true

The following options have not been explicitly set, so using the following defaults:
- alpha-quality: 85
- auto-filter: false
- preset: "none"
- size-in-percentage: null (not set)
- skip: false
- rel-path-to-precompiled-binaries: *****
------------

Encoding is set to auto - converting to both lossless and lossy and selecting the smallest file

Converting to lossy
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Quality of source could not be established (Imagick or GraphicsMagick is required) - Using default instead (70).
The near-lossless option ignored for lossy
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 70 -alpha_q '85' -m 6 -low_memory '[doc-root]/wp-content/uploads/2017/02/beetroot-quinoa2.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/02/beetroot-quinoa2.jpg.webp.lossy.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/02/beetroot-quinoa2.jpg.webp.lossy.webp'
File:      [doc-root]/wp-content/uploads/2017/02/beetroot-quinoa2.jpg
Dimension: 1200 x 800
Output:    56428 bytes Y-U-V-All-PSNR 40.92 45.63 44.39   41.90 dB
           (0.47 bpp)
block count:  intra4:       3000  (80.00%)
              intra16:       750  (20.00%)
              skipped:        10  (0.27%)
bytes used:  header:            196  (0.3%)
             mode-partition:   9780  (17.3%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
  intra4-coeffs:  |   29504 |    2828 |    1260 |     369 |   33961  (60.2%)
 intra16-coeffs:  |    1579 |     880 |     776 |     503 |    3738  (6.6%)
  chroma coeffs:  |    6783 |     978 |     634 |     330 |    8725  (15.5%)
    macroblocks:  |      69%|      14%|      10%|       7%|    3750
      quantizer:  |      32 |      23 |      16 |      16 |
   filter level:  |      34 |      20 |      19 |       7 |
------------------+---------+---------+---------+---------+-----------------
 segments total:  |   37866 |    4686 |    2670 |    1202 |   46424  (82.3%)

Success
Reduction: 16% (went from 66 kb to 55 kb)

Converting to lossless
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 70 -alpha_q '85' -near_lossless 60 -m 6 -low_memory '[doc-root]/wp-content/uploads/2017/02/beetroot-quinoa2.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/02/beetroot-quinoa2.jpg.webp.lossless.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/02/beetroot-quinoa2.jpg.webp.lossless.webp'
File:      [doc-root]/wp-content/uploads/2017/02/beetroot-quinoa2.jpg
Dimension: 1200 x 800
Output:    513298 bytes (4.28 bpp)
Lossless-ARGB compressed size: 513298 bytes
  * Header size: 4575 bytes, image data size: 508697
  * Lossless features used: PREDICTION CROSS-COLOR-TRANSFORM SUBTRACT-GREEN
  * Precision Bits: histogram=5 transform=4 cache=10

Success
Reduction: -664% (went from 66 kb to 501 kb)

Picking lossy
cwebp succeeded :)

Converted image in 1653 ms, reducing file size with 16% (went from 66 kb to 55 kb)
