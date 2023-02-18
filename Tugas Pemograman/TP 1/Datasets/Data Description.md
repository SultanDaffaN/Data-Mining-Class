# Deskripsi Fitur
## cuaca_harian.csv
* time – Tanggal pencatatan
* temperature_2m_max (°C) – Temperatur udara tertinggi pada ketinggian 2 m di atas permukaan
* temperature_2m_min (°C) – Temperatur udara terendah pada ketinggian 2 m di atas permukaan
* apparent_temperature_max (°C) – Temperatur semu maksimum yang terasa
* apparent_temperature_min (°C) – Temperatur semu minimum yang terasa
* sunrise (iso8601) – Waktu matahari terbit pada hari itu dengan format ISO 8601
* sunset (iso8601) – Waktu matahari tenggelam pada hari itu dengan format ISO 8601
* shortwave_radiation_sum (MJ/m²) – Total radiasi matahari pada hari tersebut
* rain_sum (mm) – Jumlah curah hujan pada hari tersebut
* windspeed_10m_max (km/h) – Kecepatan angin maksimum pada ketinggian 10 m
* windgusts_10m_max (km/h) - Kecepatan angin minimum pada ketinggian 10 m
* winddirection_10m_dominant (°) – Arah angin dominan pada hari tersebut
* city – Nama kota yang tercatat
* class – Jenis/kelompok curah hujan harian

## cuaca_jaman.csv
* time – Tanggal dan jam pencatatan
* temperature_2m (°C) – Temperatur pada ketinggian 2 m
* relativehumidity_2m (%) – Kelembapan pada ketinggian 2 m
* dewpoint_2m (°C) – Titik embun; suhu ambang udara mengembun
* apparent_temperature (°C) – Temperatur semu yang dirasakan
* pressure_msl (hPa) – Tekanan udara pada ketinggian permukaan air laut rata-rata (mean sea level)
* surface_pressure (hPa) – Tekanan udara pada ketinggian permukaan daerah tersebut
* snowfall (cm) – Jumlah hujan salju pada jam tersebut
* cloudcover_low (%) – Persentase cloud cover pada awan sampai ketinggian 2 km
* cloudcover_mid (%) – Persentase cloud cover pada ketinggian 2-6 km
* cloudcover_high (%) – Persentase cloud cover pada ketinggian di atas 6 km
* shortwave_radiation (W/m²) – Rata-rata energi pancaran matahari pada gelombang inframerah hingga ultraviolet
* direct_radiation (W/m²) – Rata-rata pancaran matahari langsung pada permukaan tanah seluas 1 m2
* diffuse_radiation (W/m²) – Rata-rata pancaran matahari yang dihamburkan oleh permukaan dan atmosfer
* direct_normal_irradiance (W/m²) – Rata-rata pancaran matahari langsung pada luas 1 m2 tegak lurus dengan arah pancaran
* windspeed_10m (km/h) – Kecepatan angin pada ketinggian 10 m
* windspeed_100m (km/h) – Kecepatan angin pada ketinggian 100 m
* winddirection_10m (°) – Arah angin pada ketinggian 10 m
* winddirection_100m (°) – Arah angin pada ketinggian 100 m
* windgusts_10m (km/h) – Kecepatan angin ketika terdapat angin kencang
* et0_fao_evapotranspiration (mm) – Jumlah evapotranspirasi (evaporasi dan transpirasi) pada jam tersebut
* vapor_pressure_deficit (kPa) – Perbedaan tekanan uap air dari udara dengan tekanan uap air ketika udara tersaturasi
* soil_temperature_0_to_7cm (°C) – Rata-rata temperatur tanah pada kedalaman 0-7 cm
* soil_temperature_7_to_28cm (°C) – Rata-rata temperatur tanah pada kedalaman 7-28 cm
* soil_temperature_28_to_100cm (°C) – Rata-rata temperatur tanah pada kedalaman 28-100 cm
* soil_temperature_100_to_255cm (°C) – Rata-rata temperatur tanah pada kedalaman 100-255 cm
* soil_moisture_0_to_7cm (m³/m³) – Rata-rata kelembapan air pada tanah untuk kedalaman 0-7 cm
* soil_moisture_7_to_28cm (m³/m³) – Rata-rata kelembapan air pada tanah untuk kedalaman 7-28 cm
* soil_moisture_28_to_100cm (m³/m³) – Rata-rata kelembapan air pada tanah untuk kedalaman 28-100 cm
* soil_moisture_100_to_255cm (m³/m³) – Rata-rata kelembapan air pada tanah untuk kedalaman 100-255 cm
* city – Nama kota


# RQ:
1. **Bagaimana hubungan ke empat kolom mengenai `soil_moisture` dengan jumlah curah hujan harian?** *soil_moisture kalo diambil difference lalu dikalikan dengan bobot dapat memiliki distribusi yang mirip dengan curah hujan
2. **Kota mana saja yang dekat secara geografis?** * dari curah hujan, kota si(singaraja) dan u(ubud) memiliki kemiripan
3. **Jika data di atas merupakan data yang nyata, berada di daerah manakah kota q?** *q(qeqertat) merupakan daerah di greenland. Hasil ini bisa diperoleh berdasarkan daerah yang tidak disinari matahari pada interval tanggal yang memiliki sunrise dan sunset
