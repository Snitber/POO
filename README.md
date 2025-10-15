public class CuentaBancaria {

    private String titular;jhonnier 
    private String numeroCuenta;112045714
    private double saldo20.000


    public CuentaBancaria() {
        this.titular = "Sin titular";
        this.numeroCuenta = "000000";
        this.saldo = 0.0;
    }
    public CuentaBancaria(String titular, String numeroCuenta, double saldo) {
        setTitular(titular);
        setNumeroCuenta(numeroCuenta);
        setSaldo(saldo);
    }

       public String getTitular() {
        return titular;
    }

    public void setTitular(String titular) {
        if (titular != null && !titular.trim().isEmpty()) {
            this.titular = titular;
        } else {
