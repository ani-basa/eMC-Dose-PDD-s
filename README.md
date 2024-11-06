<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>6E f100 A06 - Energy Visualization</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
        }
        .parameter-section {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 15px;
            margin: 20px auto;
            padding: 10px;
            width: 80%;
            background: #fff;
            border: 1px solid #ddd;
            border-radius: 8px;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
        }
        table {
            width: 90%;
            margin: 20px auto;
            border-collapse: collapse;
            background: #fff;
            border: 1px solid #ddd;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 10px;
            text-align: center;
        }
        img {
            width: 300px;
            height: auto;
            border: 1px solid #ccc;
            border-radius: 8px;
            cursor: pointer;
        }
        .lightbox {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }
        .lightbox img {
            width: 80%;
            max-width: 800px;
            border: 2px solid #fff;
            border-radius: 8px;
        }
        .lightbox:target {
            display: flex;
        }
    </style>
</head>
<body>
    <h1>Energy Visualization - 6E f100 A06</h1>

    <div class="parameter-section">
        <label for="energySelect"><strong>Energy:</strong></label>
        <select id="energySelect">
            <option>6E</option>
        </select>
        
        <label for="applicatorSelect"><strong>Applicator:</strong></label>
        <select id="applicatorSelect">
            <option>A06</option>
        </select>
        
        <label for="ssdSelect"><strong>SSD:</strong></label>
        <select id="ssdSelect">
            <option>100</option>
        </select>
    </div>

    <!-- Chart Table -->
    <table>
        <thead>
            <tr>
                <th>Sheet</th>
                <th>V0</th>
                <th>V1</th>
                <th>V2</th>
                <th>V3</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>6Ef100 2C</td>
                <td><a href="#v0_2C"><img src="v0_6E_f100_A06_2C_full_legend.png" alt="V0 2C"></a></td>
                <td><a href="#v1_2C"><img src="v1_6E_f100_A06_2C_styled.png" alt="V1 2C"></a></td>
                <td><a href="#v2_2C"><img src="v2_6E_f100_A06_2C_styled.png" alt="V2 2C"></a></td>
                <td><a href="#v3_2C"><img src="v3_6E_f100_A06_2C_styled.png" alt="V3 2C"></a></td>
            </tr>
            <tr>
                <td>6Ef100 3C</td>
                <td><a href="#v0_3C"><img src="v0__3C_styled.png" alt="V0 3C"></a></td>
                <td><a href="#v1_3C"><img src="v1__3C_styled.png" alt="V1 3C"></a></td>
                <td><a href="#v2_3C"><img src="v2__3C_styled.png" alt="V2 3C"></a></td>
                <td><a href="#v3_3C"><img src="v3__3C_styled.png" alt="V3 3C"></a></td>
            </tr>
            <tr>
                <td>6Ef100 4C</td>
                <td><a href="#v0_4C"><img src="v0__4C_styled.png" alt="V0 4C"></a></td>
                <td><a href="#v1_4C"><img src="v1__4C_styled.png" alt="V1 4C"></a></td>
                <td><a href="#v2_4C"><img src="v2__4C_styled.png" alt="V2 4C"></a></td>
                <td><a href="#v3_4C"><img src="v3__4C_styled.png" alt="V3 4C"></a></td>
            </tr>
            <tr>
                <td>6Ef100 5C</td>
                <td><a href="#v0_5C"><img src="v0_5C_styled.png" alt="V0 5C"></a></td>
                <td><a href="#v1_5C"><img src="v1_5C_styled.png" alt="V1 5C"></a></td>
                <td><a href="#v2_5C"><img src="v2_5C_styled.png" alt="V2 5C"></a></td>
                <td><a href="#v3_5C"><img src="v3_5C_styled.png" alt="V3 5C"></a></td>
            </tr>
            <tr>
                <td>6Ef100 Open</td>
                <td><a href="#v0_Open"><img src="v0_Open_styled.png" alt="V0 Open"></a></td>
                <td><a href="#v1_Open"><img src="v1_Open_styled.png" alt="V1 Open"></a></td>
                <td><a href="#v2_Open"><img src="v2_Open_styled.png" alt="V2 Open"></a></td>
                <td><a href="#v3_Open"><img src="v3_Open_styled.png" alt="V3 Open"></a></td>
            </tr>
        </tbody>
    </table>

    <!-- Lightbox for Each Image -->
    <div id="v0_2C" class="lightbox"><img src="v0_6E_f100_A06_2C_full_legend.png" alt="V0 2C"></div>
    <div id="v1_2C" class="lightbox"><img src="v1_6E_f100_A06_2C_styled.png" alt="V1 2C"></div>
    <div id="v2_2C" class="lightbox"><img src="v2_6E_f100_A06_2C_styled.png" alt="V2 2C"></div>
    <div id="v3_2C" class="lightbox"><img src="v3_6E_f100_A06_2C_styled.png" alt="V3 2C"></div>

    <div id="v0_3C" class="lightbox"><img src="v0__3C_styled.png" alt="V0 3C"></div>
    <div id="v1_3C" class="lightbox"><img src="v1__3C_styled.png" alt="V1 3C"></div>
    <div id="v2_3C" class="lightbox"><img src="v2__3C_styled.png" alt="V2 3C"></div>
    <div id="v3_3C" class="lightbox"><img src="v3__3C_styled.png" alt="V3 3C"></div>

    <div id="v0_4C" class="lightbox"><img src="v0__4C_styled.png" alt="V0 4C"></div>
    <div id="v1_4C" class="lightbox"><img src="v1__4C_styled.png" alt="V1 4C"></div>
    <div id="v2_4C" class="lightbox"><img src="v2__4C_styled.png" alt="V2 4C"></div>
    <div id="v3_4C" class="lightbox"><img src="v3__4C_styled.png" alt="V3 4C"></div>

    <div id="v0_5C" class="lightbox"><img src="v0_5C_styled.png" alt="V0 5C"></div>
    <div id="v1_5C" class="lightbox"><img src="v1_5C_styled.png" alt="V1 5C"></div>
    <div id="v2_5C" class="lightbox"><img src="v2_5C_styled.png" alt="V2 5C"></div>
    <div id="v3_5C" class="lightbox"><img src="v3_5C_styled.png" alt="V3 5C"></div>

    <div id="v0_Open" class="lightbox"><img src="v0_Open_styled.png" alt="V0 Open"></div>
    <div id="v1_Open" class="lightbox"><img src="v1_Open_styled.png" alt="V1 Open"></div>
    <div id="v2_Open" class="lightbox"><img src="v2_Open_styled.png" alt="V2 Open"></div>
    <div id="v3_Open" class="lightbox"><img src="v3_Open_styled.png" alt="V3 Open"></div>

    <script>
        // Close the lightbox when clicked outside of the image
        document.addEventListener('click', function(event) {
            if (event.target.classList.contains('lightbox')) {
                window.location.hash = '';  // Remove hash to close lightbox
            }
        });
    </script>
</body>
</html>
