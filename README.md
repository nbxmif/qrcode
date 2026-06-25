# QRIS Decoder and Parser

## Yang diperbaiki:

Load jsQR dari cdn.jsdelivr.net yang proper untuk standalone HTML
Tambah loading spinner saat proses decode
Coba 3 skala gambar (100%, 200%, 50%) supaya deteksi lebih robust
Error message lebih informatif

## Fitur tambahan:

Ctrl+V langsung di halaman juga bisa paste gambar (tidak perlu klik tombol paste dulu)
Tombol "Copy" untuk copy raw string
Value enriched — contoh tag 53 (currency) langsung tampil 360 → IDR – Rupiah Indonesia
Tag 01 langsung tampil apakah Static atau Dynamic QR

---
## Tag Descriptions // Define descriptions for common EMVCo/QRIS TLV tags
tag Descriptions: 
      '00': 'Payload Format Indicator',
      '01': 'Point of Initiation Method',
      '02': 'Visa Credit', // Example for Merchant Account Information (MAI)
      '03': 'Mastercard Credit', // Example for MAI
      '04': 'EMVCo Reserved', // Example for MAI
      '05': 'QRIS Merchant Criteria', // Example for MAI
      '06': 'QRIS Merchant ID', // Example for MAI
      '07': 'QRIS Terminal ID', // Example for MAI
      '08': 'QRIS Merchant Name', // Example for MAI
      '09': 'QRIS City', // Example for MAI
      '10': 'QRIS Postal Code', // Example for MAI
      '11': 'QRIS Country', // Example for MAI
      '12': 'QRIS Transaction Type', // Example for MAI
      '13': 'QRIS Reference Label', // Example for MAI
      '14': 'QRIS Consumer ID', // Example for MAI
      '15': 'QRIS Bill Number', // Example for MAI
      '16': 'QRIS Mobile Number', // Example for MAI
      '17': 'QRIS Store Label', // Example for MAI
      '18': 'QRIS Loyalty Number', // Example for MAI
      '19': 'QRIS Customer Label', // Example for MAI
      '20': 'QRIS Purpose of Transaction', // Example for MAI
      '21': 'QRIS Additional Consumer Data', // Example for MAI
      '22': 'QRIS Payment Instrument Type', // Example for MAI
      '23': 'QRIS Payment Instrument ID', // Example for MAI
      '24': 'QRIS Payment Instrument Expiry', // Example for MAI
      '25': 'QRIS Payment Instrument Holder Name', // Example for MAI
      '26': 'Merchant Account Information (Template)',
      '51': 'QRIS Merchant Information (Template)',
      '52': 'Merchant Category Code',
      '53': 'Currency Code (ISO 4217)',
      '54': 'Transaction Amount',
      '55': 'Tip or Convenience Indicator',
      '56': 'Value of Convenience Fee Fixed',
      '57': 'Value of Convenience Fee Percentage',
      '58': 'Country Code (ISO 3166-1 alpha-2)',
      '59': 'Merchant Name',
      '60': 'Merchant City',
      '61': 'Postal Code',
      '62': 'Additional Data Field (Template)',
      '63': 'CRC (Cyclic Redundancy Check)',
      '64': 'Merchant Information Language (Template)',
      '65': 'RFU for EMVCo', // Reserved for Future Use
      '66': 'RFU for EMVCo',
      '67': 'RFU for EMVCo',
      '68': 'RFU for EMVCo',
      '69': 'RFU for EMVCo',
      '70': 'RFU for EMVCo',
      '71': 'RFU for EMVCo',
      '72': 'RFU for EMVCo',
      '73': 'RFU for EMVCo',
      '74': 'RFU for EMVCo',
      '75': 'RFU for EMVCo',
      '76': 'RFU for EMVCo',
      '77': 'RFU for EMVCo',
      '78': 'RFU for EMVCo',
      '79': 'RFU for EMVCo',
      '80': 'RFU for EMVCo',
      '81': 'RFU for EMVCo',
      '82': 'RFU for EMVCo',
      '83': 'RFU for EMVCo',
      '84': 'RFU for EMVCo',
      '85': 'Merchant Information - Proprietary',
      '99': 'Unreserved Templates',
