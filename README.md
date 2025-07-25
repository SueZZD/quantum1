# Kuantum Devresi Simülasyonu
Bu proje, Qiskit kütüphanesini kullanarak basit bir kuantum devresi oluşturmayı ve görselleştirmeyi amaçlayan bir Python Jupyter Notebook'udur (veya Colab Notebook'u). Kuantum hesaplamanın temel kavramlarını, özellikle süperpozisyon ve dolaşıklığı göstermektedir.

# Özellikler
Qiskit Entegrasyonu: Kuantum devreleri oluşturmak ve manipüle etmek için IBM'in açık kaynaklı Qiskit kütüphanesini kullanır.

Kuantum Devre Çizimi: Oluşturulan kuantum devrelerini Matplotlib kullanarak görselleştirir.

Temel Kuantum Kapıları: Hadamard (H) ve CNOT (Controlled-NOT) kapılarının uygulanmasını gösterir.

Kuantum Dolaşıklığı: İki qubit arasında kuantum dolaşıklığının nasıl oluşturulduğunu örneklendirir.

# Kullanılan Teknolojiler
Python: Projenin ana programlama dili.

Qiskit: Kuantum hesaplama için Python kütüphanesi.

Matplotlib: Python'da grafikler ve görselleştirmeler oluşturmak için kullanılır.

pylatexenc: Kuantum devre çizimlerinde LaTeX notasyonunu desteklemek için kullanılır.

Google Colab (veya Jupyter Notebook): Kodun çalıştırıldığı ve sunulduğu ortam.

# Kod Açıklaması
Notebook'un içinde, her bir kod bloğunun ne anlama geldiğini ve kuantum devresinin nasıl çalıştığını açıklayan detaylı Markdown hücreleri bulunmaktadır.

!pip install qiskit: Qiskit kütüphanesini yükler.

!pip install pylatexenc: Qiskit'in çizim fonksiyonları için gerekli olan LaTeX desteğini sağlar.

from qiskit import QuantumCircuit: Kuantum devreleri oluşturmak için QuantumCircuit sınıfını içe aktarır.

circuit = QuantumCircuit(2): 2 qubit'lik boş bir kuantum devresi oluşturur.

circuit.draw(output="mpl"): Devrenin başlangıç durumunu Matplotlib kullanarak çizer.

qc = QuantumCircuit(2): Yeni bir 2 qubit'lik devre başlatır.

qc.h(0): 0. qubite Hadamard kapısı (süperpozisyon oluşturur) uygular.

qc.cx(0,1): 0. qubiti kontrol qubiti, 1. qubiti hedef qubit olarak kullanarak CNOT kapısı (dolaşıklık oluşturur) uygular.

qc.draw(output='mpl'): Kapılar uygulandıktan sonra devrenin son halini çizer.

# Gelecekteki Geliştirmeler
Daha karmaşık kuantum algoritmalarının (örn. Shor, Grover) uygulanması.

Kuantum devrelerinin simülasyon sonuçlarının analizi.

Gerçek kuantum donanımlarında (IBM Quantum Experience) devrelerin çalıştırılması.

Interaktif görselleştirmeler eklenmesi.
