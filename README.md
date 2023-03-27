# LAB7
abstract class XeMay {
  public abstract void brake();
}

class XeMayTheThao extends XeMay {
  @Override
  public void brake() {
    System.out.println("Xe máy thể thao đang phanh bằng hệ thống phanh đĩa");
  }
}

class XeMayLeoNui extends XeMay {
  @Override
  public void brake() {
    System.out.println("Xe máy leo núi đang phanh bằng hệ thống phanh cơ");
  }
}

public class Main {
  public static void main(String[] args) {
    XeMay theThao = new XeMayTheThao();
    theThao.brake(); // output: Xe máy thể thao đang phanh bằng hệ thống phanh đĩa

    XeMay leoNui = new XeMayLeoNui();
    leoNui.brake(); // output: Xe máy leo núi đang phanh bằng hệ thống phanh cơ
  }
}
