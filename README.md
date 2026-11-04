# spin-project-repo
first-repository
package frc.robot.subsystems;

import com.ctre.phoenix6.configs.TalonFXConfiguration;
import com.ctre.phoenix6.configs.TalonFXSConfiguration;
import com.ctre.phoenix6.hardware.TalonFX;

import edu.wpi.first.wpilibj2.command.SubsystemBase;


public class leftrightstopproject extends SubsystemBase{
    public Command runRightCommand () {
        return runOnce(() -> TestMotor.set(0.3))
    }
    public Command runLeftCommand () {
        return runOnce(() -> TestMotor.set(-0.3))
    }
    public Command stopMotor () {
        return runOnce(() -> TestMotor.stopMotor())
    }
} 
