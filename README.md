<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Convert images to PDF online for free. Fast, secure, and easy-to-use image to PDF converter with multiple customization options.">
    <meta name="keywords" content="image to pdf, convert images to pdf, jpg to pdf, png to pdf, free pdf converter, online pdf creator">
    <meta name="author" content="Imagify">
    <meta name="robots" content="index, follow">
    <meta property="og:title" content="Imagify - Convert Images to PDF Online">
    <meta property="og:description" content="Free online tool to convert multiple images to PDF documents quickly and easily.">
    <meta property="og:type" content="website">
     <link rel="icon" type="image/x-icon" href="file:///home/chronos/u-2f1cabebbf7b5d4bd2cd59faac554ce761e95fda/MyFiles/Downloads/logo.png" >
    <meta property="og:url" content="https://imagify.example.com">
    <link rel="canonical" href="https://imagify.example.com">
    <title>Imagify - Convert Images to PDF Online | Free Image to PDF Converter</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_ADSENSE_ID"></script>
    <style>
        :root {
            --primary: #4361ee;
            --secondary: #3f37c9;
            --accent: #4895ef;
            --light: #f8f9fa;
            --dark: #212529;
            --success: #4cc9f0;
            --warning: #f72585;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--light);
            color: var(--dark);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1.5rem;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 1.5rem;
            font-weight: 700;
        }

        .logo i {
            font-size: 1.8rem;
            color: var(--accent);
        }

        .nav-links {
            display: flex;
            gap: 1.5rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 0.5rem 1rem;
            border-radius: 4px;
        }

        .nav-links a:hover {
            background-color: rgba(255, 255, 255, 0.2);
        }

        .container {
            flex: 1;
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 1.5rem;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .hero {
            text-align: center;
            margin-bottom: 3rem;
            width: 100%;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--primary);
            background: linear-gradient(to right, var(--primary), var(--warning));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .hero p {
            font-size: 1.1rem;
            color: #555;
            max-width: 700px;
            margin: 0 auto 2rem;
        }

        .converter-container {
            background-color: white;
            border-radius: 12px;
            box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
            padding: 2rem;
            width: 100%;
            max-width: 800px;
            transition: all 0.3s ease;
        }

        .converter-container:hover {
            box-shadow: 0 12px 28px rgba(0, 0, 0, 0.15);
            transform: translateY(-2px);
        }

        .drop-area {
            border: 2px dashed var(--accent);
            border-radius: 8px;
            padding: 3rem 2rem;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-bottom: 1.5rem;
            position: relative;
            overflow: hidden;
        }

        .drop-area.highlight {
            border-color: var(--success);
            background-color: rgba(72, 149, 239, 0.05);
        }

        .drop-area i {
            font-size: 3rem;
            color: var(--accent);
            margin-bottom: 1rem;
        }

        .drop-area h3 {
            margin-bottom: 0.5rem;
            color: var(--dark);
        }

        .drop-area p {
            color: #666;
            margin-bottom: 1rem;
        }

        .btn {
            background-color: var(--primary);
            color: white;
            border: none;
            padding: 0.75rem 1.5rem;
            border-radius: 6px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }

        .btn:hover {
            background-color: var(--secondary);
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .btn-outline {
            background-color: transparent;
            border: 2px solid var(--primary);
            color: var(--primary);
        }

        .btn-outline:hover {
            background-color: var(--primary);
            color: white;
        }

        .btn-warning {
            background-color: var(--warning);
        }

        .btn-warning:hover {
            background-color: #e5177a;
        }

        .btn-success {
            background-color: var(--success);
        }

        .btn-success:hover {
            background-color: #3ab4d8;
        }

        .file-input {
            display: none;
        }

        .preview-container {
            display: none;
            margin-top: 2rem;
            width: 100%;
        }

        .preview-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1rem;
        }

        .preview-images {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 1rem;
            max-height: 400px;
            overflow-y: auto;
            padding: 0.5rem;
        }

        .image-preview {
            position: relative;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
            aspect-ratio: 1;
        }

        .image-preview img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .remove-btn {
            position: absolute;
            top: 0.5rem;
            right: 0.5rem;
            background-color: rgba(247, 37, 133, 0.8);
            color: white;
            border: none;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .image-preview:hover .remove-btn {
            opacity: 1;
        }

        .options {
            margin-top: 2rem;
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .option-group {
            flex: 1;
            min-width: 200px;
        }

        .option-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--dark);
        }

        .option-group select, .option-group input {
            width: 100%;
            padding: 0.75rem;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-size: 1rem;
        }

        .loading {
            display: none;
            text-align: center;
            margin: 2rem 0;
        }

        .spinner {
            width: 40px;
            height: 40px;
            border: 4px solid rgba(67, 97, 238, 0.2);
            border-top: 4px solid var(--primary);
            border-radius: 50%;
            animation: spin 1s linear infinite;
            margin: 0 auto 1rem;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        .action-buttons {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
            width: 100%;
        }

        .action-buttons .btn {
            flex: 1;
            justify-content: center;
        }

        /* Ad Containers */
        .ad-container {
            width: 100%;
            margin: 2rem 0;
            text-align: center;
            background-color: #f5f5f5;
            padding: 1rem;
            border-radius: 8px;
            min-height: 90px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .ad-container.horizontal {
            max-width: 728px;
            height: 90px;
        }

        .ad-container.vertical {
            max-width: 300px;
            height: 250px;
            margin: 2rem auto;
        }

        .ad-placeholder {
            color: #666;
            font-size: 0.9rem;
        }

        footer {
            background-color: var(--dark);
            color: white;
            text-align: center;
            padding: 2rem 1rem;
            margin-top: auto;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 1.5rem;
        }

        .social-links {
            display: flex;
            gap: 1.5rem;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: var(--accent);
        }

        .copyright {
            font-size: 0.9rem;
            color: #aaa;
        }

        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 1rem;
            }

            .nav-links {
                width: 100%;
                justify-content: center;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .converter-container {
                padding: 1.5rem;
            }

            .options {
                flex-direction: column;
            }

            .action-buttons {
                flex-direction: column;
            }

            .ad-container.horizontal {
                height: 100px;
            }
        }

        /* Structured Data for Rich Snippets */
        .structured-data {
            display: none;
        }
    </style>
</head>
<body>
    <header>
        <div class="navbar">
            <div class="logo">
                <i class="fas fa-file-pdf"></i>
                <span>Imagify</span>
            </div>
            <div class="nav-links">
                <a href="#" class="active">Home</a>
                <a href="#">Features</a>
                <a href="#">About</a>
                <a href="#">Contact</a>
            </div>
        </div>
    </header>

    <div class="container">
        <!-- Top Ad Banner -->
        <div class="ad-container horizontal">
            <!-- Replace with your actual ad code -->
            <ins class="adsbygoogle"
                 style="display:block"
                 data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                 data-ad-slot="1234567890"
                 data-ad-format="auto"
                 data-full-width-responsive="true"></ins>
            <script>
                 (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>

        <div class="hero">
            <h1>Convert Images to PDF in Seconds</h1>
            <p>Drag and drop your images or select files to create a professional PDF document. Fast, secure, and completely free!</p>
        </div>

        <div class="converter-container">
            <div class="drop-area" id="dropArea">
                <i class="fas fa-cloud-upload-alt"></i>
                <h3>Drag & Drop Your Images Here</h3>
                <p>or</p>
                <button class="btn" id="selectFilesBtn">
                    <i class="fas fa-folder-open"></i> Select Files
                </button>
                <input type="file" id="fileInput" class="file-input" accept="image/*" multiple>
            </div>

            <div class="preview-container" id="previewContainer">
                <div class="preview-header">
                    <h3>Selected Images</h3>
                    <button class="btn btn-warning" id="clearAllBtn">
                        <i class="fas fa-trash"></i> Clear All
                    </button>
                </div>
                <div class="preview-images" id="previewImages"></div>

                <div class="options">
                    <div class="option-group">
                        <label for="pdfName">PDF Name</label>
                        <input type="text" id="pdfName" placeholder="Enter PDF name" value="converted_images">
                    </div>
                    <div class="option-group">
                        <label for="pageSize">Page Size</label>
                        <select id="pageSize">
                            <option value="a4">A4</option>
                            <option value="letter">Letter</option>
                            <option value="legal">Legal</option>
                            <option value="auto">Auto (Fit to image)</option>
                        </select>
                    </div>
                    <div class="option-group">
                        <label for="pageOrientation">Orientation</label>
                        <select id="pageOrientation">
                            <option value="portrait">Portrait</option>
                            <option value="landscape">Landscape</option>
                        </select>
                    </div>
                </div>

                <div class="loading" id="loading">
                    <div class="spinner"></div>
                    <p>Creating your PDF...</p>
                </div>

                <div class="action-buttons">
                    <button class="btn" id="convertBtn">
                        <i class="fas fa-file-pdf"></i> Convert to PDF
                    </button>
                    <button class="btn btn-success" id="downloadBtn" style="display: none;">
                        <i class="fas fa-download"></i> Download PDF
                    </button>
                    <button class="btn btn-outline" id="newConversionBtn" style="display: none;">
                        <i class="fas fa-redo"></i> New Conversion
                    </button>
                </div>
            </div>
        </div>

        <!-- Sidebar Ad (shown on larger screens) -->
        <div class="ad-container vertical" style="display: none;">
            <!-- Replace with your actual ad code -->
            <ins class="adsbygoogle"
                 style="display:block"
                 data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                 data-ad-slot="0987654321"
                 data-ad-format="auto"
                 data-full-width-responsive="true"></ins>
            <script>
                 (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>
    </div>

    <footer>
        <div class="footer-content">
            <div class="logo">
                <i class="fas fa-file-pdf"></i>
                <span>Imagify</span>
            </div>
            <p>The easiest way to convert your images to PDF documents</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-github"></i></a>
            </div>
            <p class="copyright">© 2025 Imagify. All rights reserved.</p>
        </div>
    </footer>

    <!-- Structured Data for SEO -->
    <script type="application/ld+json" class="structured-data">
    {
        "@context": "https://schema.org",
        "@type": "WebApplication",
        "name": "Imagify - Image to PDF Converter",
        "url": "https://imagify.example.com",
        "description": "Free online tool to convert multiple images to PDF documents quickly and easily.",
        "applicationCategory": "UtilityApplication",
        "operatingSystem": "Web Browser",
        "offers": {
            "@type": "Offer",
            "price": "0",
            "priceCurrency": "USD"
        },
        "creator": {
            "@type": "Organization",
            "name": "Imagify"
        }
    }
    </script>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <script>
        // Initialize jsPDF
        const { jsPDF } = window.jspdf;

        // DOM Elements
        const dropArea = document.getElementById('dropArea');
        const fileInput = document.getElementById('fileInput');
        const selectFilesBtn = document.getElementById('selectFilesBtn');
        const previewContainer = document.getElementById('previewContainer');
        const previewImages = document.getElementById('previewImages');
        const clearAllBtn = document.getElementById('clearAllBtn');
        const convertBtn = document.getElementById('convertBtn');
        const downloadBtn = document.getElementById('downloadBtn');
        const newConversionBtn = document.getElementById('newConversionBtn');
        const loading = document.getElementById('loading');
        const pdfNameInput = document.getElementById('pdfName');
        const pageSizeSelect = document.getElementById('pageSize');
        const pageOrientationSelect = document.getElementById('pageOrientation');
        const verticalAd = document.querySelector('.ad-container.vertical');

        // Store selected files and generated PDF
        let files = [];
        let generatedPdf = null;

        // Show vertical ad on larger screens
        if (window.innerWidth > 992) {
            verticalAd.style.display = 'flex';
        }

        window.addEventListener('resize', () => {
            if (window.innerWidth > 992) {
                verticalAd.style.display = 'flex';
            } else {
                verticalAd.style.display = 'none';
            }
        });

        // Event Listeners
        selectFilesBtn.addEventListener('click', () => fileInput.click());
        fileInput.addEventListener('change', handleFileSelect);
        dropArea.addEventListener('dragover', handleDragOver);
        dropArea.addEventListener('dragleave', handleDragLeave);
        dropArea.addEventListener('drop', handleDrop);
        clearAllBtn.addEventListener('click', clearAllFiles);
        convertBtn.addEventListener('click', convertToPDF);
        downloadBtn.addEventListener('click', downloadPDF);
        newConversionBtn.addEventListener('click', startNewConversion);

        // Functions
        function handleFileSelect(e) {
            const selectedFiles = e.target.files;
            if (selectedFiles.length > 0) {
                files = Array.from(selectedFiles);
                updatePreview();
            }
        }

        function handleDragOver(e) {
            e.preventDefault();
            dropArea.classList.add('highlight');
        }

        function handleDragLeave() {
            dropArea.classList.remove('highlight');
        }

        function handleDrop(e) {
            e.preventDefault();
            dropArea.classList.remove('highlight');
            
            const droppedFiles = e.dataTransfer.files;
            if (droppedFiles.length > 0) {
                files = Array.from(droppedFiles).filter(file => file.type.startsWith('image/'));
                updatePreview();
            }
        }

        function updatePreview() {
            if (files.length === 0) return;
            
            previewImages.innerHTML = '';
            
            files.forEach((file, index) => {
                const reader = new FileReader();
                reader.onload = (e) => {
                    const imagePreview = document.createElement('div');
                    imagePreview.className = 'image-preview';
                    
                    const img = document.createElement('img');
                    img.src = e.target.result;
                    img.alt = file.name;
                    
                    const removeBtn = document.createElement('button');
                    removeBtn.className = 'remove-btn';
                    removeBtn.innerHTML = '<i class="fas fa-times"></i>';
                    removeBtn.addEventListener('click', () => removeFile(index));
                    
                    imagePreview.appendChild(img);
                    imagePreview.appendChild(removeBtn);
                    previewImages.appendChild(imagePreview);
                };
                reader.readAsDataURL(file);
            });
            
            previewContainer.style.display = 'block';
            showConvertButton();
        }

        function removeFile(index) {
            files.splice(index, 1);
            updatePreview();
            
            if (files.length === 0) {
                previewContainer.style.display = 'none';
            }
        }

        function clearAllFiles() {
            files = [];
            previewContainer.style.display = 'none';
            fileInput.value = '';
            generatedPdf = null;
            showConvertButton();
        }

        function showConvertButton() {
            convertBtn.style.display = 'flex';
            downloadBtn.style.display = 'none';
            newConversionBtn.style.display = 'none';
        }

        function showDownloadButtons() {
            convertBtn.style.display = 'none';
            downloadBtn.style.display = 'flex';
            newConversionBtn.style.display = 'flex';
        }

        async function convertToPDF() {
            if (files.length === 0) {
                alert('Please select at least one image to convert.');
                return;
            }

            // Show loading
            loading.style.display = 'block';
            convertBtn.disabled = true;

            // Get user options
            const pdfName = pdfNameInput.value || 'converted_images';
            const pageSize = pageSizeSelect.value;
            const orientation = pageOrientationSelect.value;

            // Create PDF
            const pdf = new jsPDF({
                orientation: orientation,
                unit: 'mm',
                format: pageSize === 'auto' ? undefined : pageSize
            });

            try {
                // Process each image
                for (let i = 0; i < files.length; i++) {
                    const file = files[i];
                    const imgData = await readFileAsDataURL(file);
                    
                    if (i > 0) {
                        pdf.addPage();
                    }
                    
                    // Add image to PDF
                    if (pageSize === 'auto') {
                        // Get image dimensions to fit the page
                        const img = await loadImage(imgData);
                        const imgWidth = img.width;
                        const imgHeight = img.height;
                        
                        // Calculate dimensions to fit PDF (A4 ratio)
                        const pdfWidth = pdf.internal.pageSize.getWidth();
                        const pdfHeight = pdf.internal.pageSize.getHeight();
                        
                        let width, height;
                        const imgRatio = imgWidth / imgHeight;
                        const pdfRatio = pdfWidth / pdfHeight;
                        
                        if (imgRatio > pdfRatio) {
                            width = pdfWidth;
                            height = pdfWidth / imgRatio;
                        } else {
                            height = pdfHeight;
                            width = pdfHeight * imgRatio;
                        }
                        
                        pdf.addImage(imgData, 'JPEG', 0, 0, width, height);
                    } else {
                        // Fit to selected page size
                        pdf.addImage(imgData, 'JPEG', 0, 0, pdf.internal.pageSize.getWidth(), pdf.internal.pageSize.getHeight());
                    }
                }
                
                // Store the generated PDF
                generatedPdf = pdf;
                
                // Show download button instead of convert button
                showDownloadButtons();
                
            } catch (error) {
                console.error('Error creating PDF:', error);
                alert('An error occurred while creating the PDF. Please try again.');
            } finally {
                // Hide loading
                loading.style.display = 'none';
                convertBtn.disabled = false;
            }
        }

        function downloadPDF() {
            if (generatedPdf) {
                const pdfName = pdfNameInput.value || 'converted_images';
                generatedPdf.save(`${pdfName}.pdf`);
            }
        }

        function startNewConversion() {
            clearAllFiles();
        }

        function readFileAsDataURL(file) {
            return new Promise((resolve, reject) => {
                const reader = new FileReader();
                reader.onload = () => resolve(reader.result);
                reader.onerror = reject;
                reader.readAsDataURL(file);
            });
        }

        function loadImage(src) {
            return new Promise((resolve, reject) => {
                const img = new Image();
                img.onload = () => resolve(img);
                img.onerror = reject;
                img.src = src;
            });
        }
    </script>
</body>
</html>
